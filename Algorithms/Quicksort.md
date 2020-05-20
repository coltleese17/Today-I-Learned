# Quicksort


Quicksort can be used for selction i.e. given an array of N items, find a kth smallest item.
quick select takes linear time on average. some how, is a variant of quicksort.

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

Sort Phase
```
static void sort(comp[] a)
StdRandom.shuffle(a);
sort(a,0,a.length-1)

static void sort(comp[] a, int lo, int hi){
if (hi <= lo) return;
int j = partition(a, lo, hi);
sort(a, lo, j-1);
sort(a, j+1, h1);
}


Time complexity is (nlogn)
it is not stable. can improve the sort by instead doing insertion sort for small cases. cutoff is roughly 10
if hi <= lo + cutoff -1)
{
insertion.sort(a.lo.hi);
return;
}
