# code-runner-li60
Code running API for LPA

```
function send_code_to_run (body, language) {
  var formData = {
    'code_body': body,
    'language' : language
  };
  var options = {
    'method' : 'post',
    'muteHttpExceptions': true,
    "headers": {
		"content-type": "application/x-www-form-urlencoded"
			},
    'payload' : formData
  };
  const result = UrlFetchApp.fetch('https://[docker.app]/run_code', options);
  }



```
