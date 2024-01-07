<html>
<head>
  <style>
  </style>
</head>
<body>
  <h1>GIT CHEAT SHEET</h1>
  <h2>STAGE & SNAPSHOT</h2>
  <p>Working with snapshots and the Git staging area</p>
  <table>
    <tr>
      <td class="command">git status</td>
      <td class="description">show modified files in working directory, staged for your next commit</td>
    </tr>
    <tr>
      <td class="command">git add [file]</td>
      <td class="description">add a file as it looks now to your next commit (stage)</td>
    </tr>
    <tr>
      <td class="command">git reset [file]</td>
      <td class="description">unstage a file while retaining the changes in working directory</td>
    </tr>
    <tr>
      <td class="command">git diff</td>
      <td class="description">diff of what is changed but not staged</td>
    </tr>
    <tr>
      <td class="command">git diff --staged</td>
      <td class="description">diff of what is staged but not yet commited</td>
    </tr>
    <tr>
      <td class="command">git commit -m “[descriptive message]”</td>
      <td class="description">commit your staged content as a new commit snapshot</td>
    </tr>
  </table>
  <h2>SETUP</h2>
  <p>Configuring user information used across all local repositories</p>
  <table>
    <tr>
      <td class="command">git config --global user.name “[firstname lastname]”</td>
      <td class="description">set a name that is identifiable for credit when review version history</td>
    </tr>
    <tr>
      <td class="command">git config --global user.email “[valid-email]”</td>
      <td class="description">set an email address that will be associated with each history marker</td>
    </tr>
    <tr>
      <td class="command">git config --global color.ui auto</td>
      <td class="description">set automatic command line coloring for Git for easy reviewing</td>
    </tr>
  </table>
  <h2>SETUP & INIT</h2>
  <p>Configuring user information, initializing and cloning repositories</p>
  <table>
    <tr>
      <td class="command">git init</td>
      <td class="description">initialize an existing directory as a Git repository</td>
    </tr>
    <tr>
      <td class="command">git clone [url]</td>
      <td class="description">retrieve an entire repository from a hosted location via URL</td>
    </tr>
  </table>
  <h2>BRANCH & MERGE</h2>
  <p>Isolating work in branches, changing context, and integrating changes</p>
  <table>
    <tr>
      <td class="command">git branch</td>
      <td class="description">list your branches. a * will appear next to the currently active branch</td>
    </tr>
    <tr>
      <td class="command">git branch [branch-name]</td>
      <td class="description">create a new branch at the current commit</td>
    </tr>
    <tr>
      <td class="command">git checkout</td>
      <td class="description">switch to another branch and check it out into your working directory</td>
    </tr>
    <tr>
      <td class="command">git merge [branch]</td>
      <td class="description">merge the specified branch’s history into the current one</td>
    </tr>
    <tr>
      <td class="command">git log</td>
      <td class="description">show all commits in the current branch’s history</td>
    </tr>
  <h3>SHARE & UPDATE</h3>
  <p>Retrieving updates from another repository and updating local repos</p>   
  <table>
    <tr>
      <td class="command">git remote add [alias] [url]</td>
      <td class="description">add a git URL as an alias</td>
    </tr>
    <tr>
      <td class="command">git fetch [alias]</td>
      <td class="description">fetch down all the branches from that Git remote</td>
    </tr>
    <tr>
      <td class="command">git merge [alias]/[branch]</td>
      <td class="description">merge a remote branch into your current branch to bring it up to date</td>
    </tr>
    <tr>
      <td class="command">git push [alias] [branch]</td>
      <td class="description">Transmit local branch commits to the remote repository branch</td>
    </tr>
    <tr>
      <td class="command">git pull</td>
      <td class="description">fetch and merge any commits from the tracking remote branch</td>
    </tr>
  </table>
  <h2>TRACKING PATH CHANGES</h2>
  <p>Versioning file removes and path changes</p>
  <table>
    <tr>
      <td class="command">git rm [file]</td>
      <td class="description">delete the file from project and stage the removal for commit</td>
    </tr>
    <tr>
      <td class="command">git mv [existing-path] [new-path]</td>
      <td class="description">change an existing file path and stage the move</td>
    </tr>
    <tr>
      <td class="command">git log --stat -M</td>
      <td class="description">show all commit logs with indication of any paths that moved</td>
    </tr>
  </table>
  <h2>TEMPORARY COMMITS</h2>
  <p>Temporarily store modified, tracked files in order to change branches</p>
  <table>
    <tr>
      <td class="command">git stash</td>
      <td class="description">Save modified and staged changes</td>
    </tr>
    <tr>
      <td class="command">git stash list</td>
      <td class="description">list stack-order of stashed file changes</td>
    </tr>
    <tr>
      <td class="command">git stash pop</td>
      <td class="description">write working from top of stash stack</td>
    </tr>
    <tr>
      <td class="command">git stash drop</td>
      <td class="description">discard the changes from top of stash stack</td>
    </tr>
  </table>
  <h2>REWRITE HISTORY</h2>
  <p>Rewriting branches, updating commits and clearing history</p>
  <table>
    <tr>
      <td>