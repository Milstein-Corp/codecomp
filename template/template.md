# How to use the templates
Refer to [google.md](../google.md) for comments on the various competitive programming platform, this document details on how to use the templates.



Specify a problem ID, open one terminal tab per question.

```bash
export PROBLEM_ID=a
```

Copy the template

```bash
cp sample.py $PROBLEM_ID.py
cp sample $PROBLEM_ID
```

Run the template, or simply `p a.py < a`

```bash
python3 $PROBLEM_ID.py < $PROBLEM_ID
```



### Preflight checklist

Activate environment `ss; sa code`

Open a jupyter notebook `jn`

Open VSCode `code .`

Reset in the template folder



## Interactive problems

Run this on your computer to ensure that it is working

```bash
for TEST_CASE in 0 1 2
do
  python interactive_runner.py python3 sample_local_testing_tool.py $TEST_CASE -- python3 sample_interactive_script.py
done
```



For competition usage

```bash
for TEST_CASE in 0 1 2
do
  python interactive_runner.py python3 local_testing_tool.py $TEST_CASE -- python3 interactive.py
done
```

