# Your first pull request

We do this together in your team's first weekly meeting. By the end you'll have added yourself to your team's repo the same way every BSD contribution works: **issue → branch → commit → pull request → review → merge.**

Your task is the issue titled **"First PR: add yourself to the team (Your Name)"** in your team's repo (e.g. `athletics-womens-field-hockey`). You'll create one small file about yourself.

## Before the meeting (5 minutes)

1. **Accept your GitHub invite** to Brown-Sports-Data: check your Brown email, or go to https://github.com/orgs/Brown-Sports-Data/invitation.
2. Open your team repo on github.com and check you can see the **Issues** tab. If you get a 404, the invite hasn't been accepted yet.

## The file you'll add

`members/<firstname>-<lastname>.md`, for example `members/justine-kang.md`:

```markdown
# Justine Kang

- **Class year:** 2027
- **Concentration:**
- **GitHub:** @justinekang
- **Project(s):** Women's Field Hockey data analysis
- **What I want to learn or build this semester:**
```

Keep it to this. No phone numbers, no data, no logins.

## Option A: in the browser (no installs)

1. Open your team repo, then **Add file → Create new file**.
2. Name it `members/<firstname>-<lastname>.md` (typing the `/` creates the folder) and paste the template above, filled in.
3. Click **Commit changes…**, choose **"Create a new branch for this commit and start a pull request"**, and name the branch `<firstname>/first-pr`.
4. Click **Propose changes**.
5. In the pull request description, write `Closes #<your issue number>`. Click **Create pull request**.

## Option B: in the terminal (how you'll work from now on)

```bash
git clone https://github.com/Brown-Sports-Data/<team-repo>.git
cd <team-repo>
git checkout -b <firstname>/first-pr
mkdir -p members
# create members/<firstname>-<lastname>.md in VS Code and fill in the template
git add members/
git commit -m "Add <Firstname> to the team"
git push -u origin <firstname>/first-pr
```

Then open the link Git prints (or the repo page → **Compare & pull request**), write `Closes #<your issue number>` in the description, and click **Create pull request**.

**Can't push?** GitHub doesn't accept your account password in the terminal. Install the GitHub CLI and run `gh auth login`, or use GitHub Desktop, then push again.

## After you open it

- Your team lead (or Alexios in the first meeting) reviews it and **squash-merges** it. Your issue closes automatically.
- Then update your copy: `git checkout main && git pull`.

That's the whole loop. Every task from here on is the same: take an issue, branch, commit, open a pull request with `Closes #…`, get it reviewed, merge. See `CONTRIBUTING.md` in your team repo for the details.
