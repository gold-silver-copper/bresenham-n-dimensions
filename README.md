# bresenham_n_dimensions
n-dimensional bresenham algorithim utilizing numpy that i found online

found it posted somewhere, i fixed a typo in a test and also modified it to include the starting point in the resulting array

look at ndbresen.py section ' if __name__ == "__main__": ' for an example of usage, for some reason you have to double bracket the starting and ending arrays

otherwise download file to same directory as python script and do

' from ndbresen import bresenhamline '

then something like

    start = np.array([[0, 0, 0]])
    end = np.array([[20, 50, 10]])
    ListOfPoints = bresenhamline(start, end,max_iter=-1)

result is

[[ 0  0  0]
 [ 0  1  0]
 [ 1  2  0]
 [ 1  3  1]
 [ 2  4  1]
...
 [20 49 10]
 [20 50 10]]
