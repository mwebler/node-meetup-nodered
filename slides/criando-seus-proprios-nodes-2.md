## Criando seus próprios nodes

`node.html`
```html
<script type="text/javascript">
    RED.nodes.registerType('lower-case',{
        category: 'function',
        color: '#a6bbcf',
        defaults: { name: {value:""} },
        inputs:1, outputs:1,
        icon: "file.png",
        label: "lower-case" });
</script>
<script type="text/x-red" data-template-name="lower-case">
    <div class="form-row">
        <label for="node-input-name"><i class="icon-tag"></i> Name</label>
        <input type="text" id="node-input-name" placeholder="Name">
    </div>
</script>
<script type="text/x-red" data-help-name="lower-case">
    <p>A simple node that converts the message to lower case</p>
</script>
```
