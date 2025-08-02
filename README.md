# LinearSearch-in-C++
#include <bits/stdc++.h>
using namespace std;

int LinearSearch(int arr[], int sz, int target)
{
    for (int i = 0; i < sz; i++)
    {
        if (arr[i] == target)
        {
            return i; // Return index if found
        }
    }
    return -1; // Return -1 if not found
}

int main()
{
    int sz;
    cout << "Enter size of the array: ";     
    cin >> sz;

    int arr[sz];  // User-defined array
    cout << "Enter " << sz << " elements: ";
    for (int i = 0; i < sz; i++)
    {
        cin >> arr[i];
    }

    int target;
    cout << "Enter the element to search: ";
    cin >> target;

    int result = LinearSearch(arr, sz, target);

    if (result != -1)
        cout << "Element found at index: " << result << endl;
    else
        cout << "Element not found in the array." << endl;

    return 0;
}


















