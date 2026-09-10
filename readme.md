# Explaination
## Commands
### git add . 
Stage everything for the commit

### git commit -m
Create a commit message

### git push 
Push everything to github

### git checkout -b <**Branch name**>
Create the new branch and move the pointer to it

### git checkout <**Branch name**>
Move the pointer to available branch

### git status
Checking the current branch that im working on

### git merge <**Branch name**>
Merge the wanted branch to the current branch

---

## Merge conflict
### Why merge conflict happened?
In branch A we specified the condition to withdrawl, in branch B we didn't add that condition but working on $2 fees. 2 branches end up being entirely different, having no similarity. Normally the old code will be replaced by new code, Git detected the conflict but could not automatically fix it so notified me.

### How did I resolve conflict?
When received notification about merge conflict I reviewed the conflicted lines and planned for change. After finished planning, I removed entire conflicting section and added new line which combine both version of code. My planned was instead of checking the balance after withdrawl to satisfy $50 threshhold, I also check if it can cover $2 fee, before adding that $2 fee in every transaction that fit the condition.