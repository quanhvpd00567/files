# vt-alert

## Include element
### To page HTML

element html input search 
```
<input type="text" id="input-search" class="form-control" placeholder="search...." />
```
element html list user
```
    <vt-users-list id='list-user' url="https://www.felixsante.com/dev/tmp/api/vt-alerts/sample1.json" keyword="" /> 
```
Javascript Listent event search
```
    


<script>
    let elem = document.getElementById('input-search');
    elem.addEventListener('input', function () {
    document.getElementById('list-user').setAttribute('keyword', elem.value)
    })
</script>

```


### To page Vue
```
    <vt-users-list :url="'https://www.felixsante.com/dev/tmp/api/vt-alerts/sample1.json'" :keyword="keyword" /> 
```
url is link api data

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
