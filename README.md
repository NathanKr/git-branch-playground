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
    <td>show local branches. The green is the current one we are working at</td>
  </tr>
  <tr>
    <td>git branch -b branch_name></td>
    <td>create a new branch from the current branch</td>
  </tr>
  <tr>
    <td>git checkout branch_name></td>
    <td>start working on branch_name</td>
  </tr>
</table>
