# Html-Table-CodingDojo
### Python - Flask - Fundamental
### Install packages
* ```pipenv install flask```
* ```pipenv shell```
* ```python server.py```
### project structure flask 
| routs           | Funtions     | return                                    |
|-----------------|--------------|-------------------------------------------|
| Localhost:5000/ | show_table() | render_template("index.html",users=users) |
### Jinja - html
```
<table>
    <thead class="table-head">
        <tr>
            <th>FirstName</th>
            <th>LastName</th>
            <th>FullName</th>
        </tr>
    </thead>
    <tbody>
        {% for user in users %}
        <tr>
            <td>{{user['first_name']}}</td>
            <td>{{user['last_name']}}</td>
            <td>{{user['first_name']}} {{user['last_name']}}</td>
        </tr>    
        {% endfor %}
    </tbody>
</table>
```
