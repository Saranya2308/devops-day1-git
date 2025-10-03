# devops-day1-git
# Day 1 – Git Mini Project

## 🎯 Objective
- Practice Git basics: init, commit, branch, merge, push  
- Simulate troubleshooting scenarios (merge conflict, commit recovery)

---

## 🛠️ Steps Done
1. Initialized Git repo with `app.py`
2. Created a `feature-logging` branch and added logging
3. Merged branch back into `main`
4. Pushed repo to GitHub

---

## ⚡ Troubleshooting Practiced
- **Merge Conflict**  
  - Edited the same line in `main` and `feature-logging`
  - On merge → conflict occurred
  - Fixed by manually editing file, then:  
    ```bash
    git add app.py
    git commit -m "Resolved merge conflict"
    ```

- **Recover Lost Commit**  
  - Deleted a commit using:  
    ```bash
    git reset --hard HEAD~1
    ```  
  - Recovered it with:  
    ```bash
    git reflog
    git checkout <commit-hash>
    ```

---

## 📚 Learnings
- Git branching helps isolate features  
- Merge conflicts are normal in teamwork — solved by manual edits  
- `git reflog` is a lifesaver for recovering commits  

---

## 🚀 Next Steps
Day 2 → Advanced Git commands (`revert`, `stash`, `reset`) with troubleshooting.
