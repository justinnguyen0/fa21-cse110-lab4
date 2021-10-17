1. The bug was that the input parameters stayed as string values, so when they were added together, string concatenation occurred instead of actually adding the numbers together.
2. I fixed the problem by converting both of the input parameters to Number when they were being added together.
![Fix](/explore/devtools/fix.png)