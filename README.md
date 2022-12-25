<h2>Motivation</h2>
Working with the master(main) branch might not be enough when working with few developers or going to production. In general you want a master(main) branch used for production and development branch used for development. Once the development is finish you merge the development branch to the master branch. So how to do it

<h2>Important commands</h2>
 <table>
  <tr>
    <th>Command</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>git branch</td>
    <td>show local branches</td>
  </tr>
  <tr>
    <td>git branch -a</td>
    <td>show local and remote branches. The green is the current one we are working at</td>
  </tr>
  <tr>
    <td>git branch -b branch_name</td>
    <td>create a new branch from the current branch</td>
  </tr>
  <tr>
    <td>git checkout branch_name</td>
    <td>start working on branch_name</td>
  </tr>
  <tr>
    <td>git branch -d branch_name</td>
    <td>delete branch locally. You can not be on the branch to delete it. If it is not merged you will not be able to delete. so either mergae or perform git branch -D dev</td>
  </tr>
  <tr>
    <td>git branch -r</td>
    <td>show remote branch</td>
  </tr>
</table>

<h2>Common flow</h2>
<ol>
<li>create once a dev branch from main using e.g 'git branch dev'</li>
<li>move to dev using 'git checkout dev'</li>
<li>make code change on the current branch (dev) and use 'git add -A' , 'git commit -m ...'</li>
<li>push to the remote dev branch using 'git push origin dev'</li>
<li>after all changes are done in dev and you want to merge to main : 'git checkout main' , 'git merge dev'</li>
<li>after merge to main it is common to delete dev </li>
</ol>