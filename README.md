# Postmark API for Spaghetti Framework

# Example
```
$postmark = new Postmark(
    'postmark-api-key,
    'From Name <from@name.com>,
    'email@reply.com'
);

$return = $postmark->to('Your name <your@email.com>')
    ->subject('Set your subject')
    ->viewData(array(
        'type' => 'something',
        'data' => $user	
    ))
    ->load_view('view_folder/template.htm')
    ->send();
```