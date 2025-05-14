程式碼在這邊，我就全部列出來了


array = [33, 67, 8, 13, 54, 119, 3, 84, 25, 41]

def BubbleSort(array):
  n = len(array) #　先定義ｎ是整個陣列的長度
  for i in range(n, 0, -1):#　ｉ的概念是要比較的趟數，即ｉ＝８時會比較前面７個數字並把最大的數字推到最右邊，並以此類推直到ｉ＝１時就把所有東西比較完了
    for j in range(0, i - 1): #　ｊ的概念就是陣列中數字的位置，因此比較時都是ｊ和ｊ＋１比較，即一個數字會和他的右邊那個數字來比較
      if (array[j] > array[j + 1]):#　所以當左邊的數字比較大的時候，就把左右兩邊交換，把大的數字一直換到最右邊
        array[j], array[j + 1] = array[j + 1], array[j]
        print("目前排序中的陣列為" , array)

BubbleSort(array)      
print("排序過後的陣列是" , array)
