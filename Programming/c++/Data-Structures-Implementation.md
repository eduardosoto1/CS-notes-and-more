# Multidimensional Arrays

- A two-dimensional array should be used to store a matrix or a table.
- Used to store data in a grid format

```cpp
// Example
double distances[8][8] = 
{
	{0, 983, 787, 714, 1375, 967, 1087},
	{983, 0, 214, 1102, 1763, 1723, 1842},
	{787, 214, 0, 888, 1549, 1548, 1627}, 
};

// Note that you can use more than a two-dimensional array!
// Example
double scores[5][8][8]; 
```

![Distances between cities table](../../../images/figure1.PNG "Distances between cities")

Fig 1.1 A table that describes the distances between several cities (illustrative example).

### Declaring Multidimensional Arrays

- An element can be accessed by going through a row and column index

```cpp
syntax is elementType arrayName[ROW_SIZE][COLUMN_SIZE]
```

<!-- The original link referenced an attachment: attachment:02f790d9-107d-4650-a9de-e69ffaeb2c8c:Capture.png which does not exist in the repo.
	Place an actual image in images/ (e.g., array2d.png) and update the path below, or keep the placeholder alt text. -->
<!-- If you add array2d.png to images/, rename the next src accordingly. -->
<img src="../../../images/figure1.PNG" alt="Two-dimensional array element indexing illustration" width="420" />

Fig 1.2 A two-dimensional array showing each element accessible (placeholder image reused; replace when new diagram added).

- If I were to add an integer 10 to column 4 and row 2, I would use

```cpp
int matrix[2][4] = 10;
```

### Initializing Arrays

- An array initializer can both declare and initialize a multidimensional array. For example

```cpp
int m[2][3] = 
{
	{1, 2, 3},
	{4, 5, 6}, 
};

// Try this
// What is m[0][2];
```

### Processing Multi-dimensional Arrays

- Nested for loops can be used to access elements
    - Instantiate arrays with values
    - Displaying Arrays
    - Performing calculations

```cpp
// For i = row and j = column;

cout << "Enter " << ROW_SIZE << " rows and " << COLUMN_SIZE << " columns: " << endl;
for (int i = 0; i < ROW_SIZE; i++)
	for (int j = 0; j < COLUMN_SIZE; j++)
	{
		// Input 
		cin >> matrix[i][j];
		
		// Output 
		cout << matrix[i][j] << " ";
	}
	cout << endl;
```