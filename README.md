# Forgetting-Machine
A Machine that forgets what happened.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Can you forget that, machine?" \
  | uvx forgetting-machine \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
pip install forgetting-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
forgetting-machine multilogue.txt
```
Or:
```bash
forgetting-machine multilogue.txt new_turn.txt
```
Or:
```bash
cat multilogue.txt | forgetting-machine
```
Or:
```bash
cat multilogue.txt | forgetting-machine > multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: Forget about ..., machine.") \
  | forgetting-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | forgetting-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | forgetting-machine > multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | forgetting-machine \
  | memory-machine > corrected_memories.md
```

Or use it in your Python code:
```Python
# Python
import forgetting_machine
```
