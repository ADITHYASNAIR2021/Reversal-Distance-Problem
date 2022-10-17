# Reversal-Distance-Problem
The problem of sorting by reversal distance is applicable primarily to the study of evolutionary distance. Determining how closely related two organisms from different species are is performed primarily by finding the minimum number of genomic reversals needed to transform one genome to the other.

This is because most inherited genomic rearrangements occurring through mutation are reversals of portions of the genome.

Finding the minimum number of such reversals that would have to take place for one genome to transform into another is therefore a good measure of the relatedness of species. It has proved to be far more effective than examining phenotypical similarities such as appearance and behaviour.

The reversal distance problem is defined as such:

Given two sequences, a and b, find the minimum number of reversals that will transform a such that it equals b.


         Here’s an example, using the numbers 1 to 9:

         a = 1, 2, 3, 4, 5, 6, 7, 8, 9

         b = 1, 2, 7, 6, 5, 4, 3, 8, 9


The problem is represented as the reordering of number sequences because this is an easier way to represent the genome than with gene names or raw DNA strings.

Each number represents a specific gene, with the same number representing the same gene in both sequences.

A reversal is an operation that takes any subsequence in sequence a, reverses the subsequence’s order, then reinserts the subsequence back into the same position.

         A reversal in our example could be:

         a = 1, 2, 3, 4, 5, 6, 7, 8, 9

         areversal = 1, 2, 4, 3, 5, 6, 7, 8, 9

In this reversal, we have simply swapped the 3 and 4 around.

Another example could be:

         a = 1, 2, 3, 4, 5, 6, 7, 8, 9

         areversal = 1, 2, 3, 9, 8, 7, 6, 5, 4

Here, we have swapped the entire subsequence after the number 3.

One more to hammer it home:

         a = 1, 2, 3, 4, 5, 6, 7, 8, 9

         areversal = 9, 8, 7, 6, 5, 4, 3, 2, 1

Here, we have taken the entire sequence as a subsequence and reversed it.

Now, the astute among you may have already worked out that the reversal distance between a and b can easily be done by hand.

         a = 1, 2, 3, 4, 5, 6, 7, 8, 9

         b = 1, 2, 7, 6, 5, 4, 3, 8, 9

         areversal = 1, 2, 7, 6, 5, 4, 3, 8, 9 = b

We only have to perform one reversal to transform a into b. Therefore, in our example, the reversal distance is 1.

