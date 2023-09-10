# example-api  
Options -MultiViews  
    RewriteEngine On  
    RewriteCond %{REQUEST_FILENAME} !-f  
    RewriteRule ^ index.html [QSA,L]  
  
app.get('/fruit/:one&:two', function(req, res) {  
    console.log(req.params.one, req.params.two)  
});  
