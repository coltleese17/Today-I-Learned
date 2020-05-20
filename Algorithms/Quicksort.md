# Quicksort

Shuffle the array.
Partionin
Sort each piece recursively

Partitioning Phase:
* repeat until I and J pointers cross.
* scan I from left to right so long as a[i] < a[lo]
* scan J from right to left so long as a[j] < a[lo]
* exchange a[i] with a[j]

```
static int partition(comp[] a, int lo, int hi){
int i = lo, j = hi+1;
while (true) {
while (less(a[++i], a[lo]))
    if (i == hi) break
while (less(a[++i], a[--j]))
    if (j == lo) break;

if (i >= j) break
exch(a,i,j)
}

exch(a,lo,j);
return j;
```

