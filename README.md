Please give it a Star if you like the project 🎉 ❤️ 

# EkoDB - A NoSQL Database made using PHP

EkoDB is a simple flat file NoSQL like database implemented in PHP without any third-party dependencies that store data in plain JSON files.

It is not designed to handle heavy-load IO operations, it is designed to have a simple solution where all we need a database for managing a few gigabytes of data. You can think of it as a database for low to medium operation loads.

## Features

- ⚡ **Lightweight, faster**

  Stores data in plain-text utilizing JSON format, no binary conversion needed to store or fetch the data. Default query cache layer.

- 🔆 **Schema free data storage**

  EkoDB does not require any schema, so you can insert any types of data you want.

- 🔍 **Query on nested properties**

  It supports schema free data, so you can filter and use conditions on nested properties of the JSON documents!

  ```php
  where( 'post.author.role', '=', 'admin' )
  ```

  EkoDB will look for data at:

  ```php
  {
    "post": {
      "author": {
        "role": "admin"
      }
    }
  }
  ```

- ✨ **Dependency free, only needs PHP to run**

  Supports PHP 7+. Requires no third-party plugins or software.

- 🚀 **Default caching layer**

  EkoDB will serve data from cache by default and regenerate cache automatically! Query results will be cached and later reused from a single file instead of traversing all the available files.

- 🌈 **Rich Conditions and Filters**

  Use multiple conditional comparisons, text search, sorting on multiple properties and nested properties. Some useful methods are:

  <table>
  <tbody>
    <tr>
      <td valign="top">
        <ul>
          <li>where</li>
          <li>orWhere</li>
          <li>select</li>
          <li>except</li>
          <li>in</li>
          <li>not in</li>
        </ul>
      </td>
      <td valign="top">
        <ul>
          <li>join</li>
          <li>like</li>
          <li>sort</li>
          <li>skip</li>
          <li>orderBy</li>
          <li>update</li>
        </ul>
      </td>
      <td valign="top">
        <ul>
          <li>limit</li>
          <li>search</li>
          <li>distinct</li>
          <li>exists</li>
          <li>first</li>
          <li>delete</li>
        </ul>
      </td>
      <td valign="top">
        <ul>
          <li>like</li>
          <li>not lik</li>
          <li>between</li>
          <li>not between</li>
          <li>group by</li>
          <li>having</li>
        </ul>
      </td>
    </tr>
  </tbody>
  </table>

- 👍 **Process data on demand**
  
  EkoDB does not require any background process or network protocol in order to process data when you use it in a PHP project. All data for a query will be fetched at runtime within the same PHP process.

- 😍 **Runs everywhere**
  
  Runs perfectly on shared-servers or VPS too.


- 🍰 **Easy to learn and implement**

  EkoDB provides a very simple elegant API to handle all of your data.

- 🍰 **Easily import/export or backup data**
  
  EkoDB use files to store information. That makes tasks like backup, import and export very easy.

- 💪 **Actively maintained**

  <p>EkoDB is created by <a rel="noopener nofollow" href="https://twitter.com/_bekiryazgann" target="_blank">@_bekiryazgann</a> who is using it in various types of applications which are in production right now.
