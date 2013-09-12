# Flows




### User loads App
```

```

### User registers
```


```
![Diagram](http://www.websequencediagrams.com/cgi-bin/cdraw?lz=dGl0bGUgUmVnaXN0ZXIKCkFwcC0-U3RhckJ1cnN0OiB1c2VybmFtZQpub3RlIHJpZ2h0IG9mIAAPEyBsb29rdXAKADQJLT5BcHA6IGV4aXN0cyBvciBubwBVC0R1AFMMLCBwYXNzd29yZCwgZW1haWwAXRMALAZjcmVhdGUACAkuVXNlci5BcAByBkR1AG4JABARLlVSTACBRhoAcAcsACEXAIFlGQCBCAd1c2VyAIIJGnNlbmQgdmVyaWZ5AIFXBwoAgkEPAIIlBXVzZXIgY2xpY2tzACcHVVJMIGluAIILBwCDCxBjb2QAgnwbAIJBBQBvBmllZAoK&s=napkin)




### User logs in
```


```
![Diagram](http://www.websequencediagrams.com/cgi-bin/cdraw?lz=dGl0bGUgTG9naW4KCkFwcC0-U3RhckNvcmU6IHVzZXJuYW1lCm5vdGUgcmlnaHQgb2YgABcKbG9va3VwACMFCgAvCC0-QXBwADYGLlN0YXJEdXN0LnVybABTCkR1c3QAUwosIHBhc3N3b3JkAFQTACUGYXV0aGVudGljYXRlAGMFRHVzdABhB2Nvb2tpZQo&s=napkin)



### User saves [dust]
```


```
![Diagram](http://www.websequencediagrams.com/cgi-bin/cdraw?lz=dGl0bGUgQ3JlYXRlIER1c3QKCkFwcC0-bG9jYWwuUG91Y2hEQjogZHVzdAoABw0tPlN0YXJEdXN0LkMAHghzeW5jCgoKCgo&s=napkin)


### User shares [dust]
```


```
![Diagram](http://www.websequencediagrams.com/cgi-bin/cdraw?lz=dGl0bGUgU2hhcmUgRHVzdAoKQXBwLT5TdGFyRHVzdDogZHVzdElELCByZWNpcGllbnQKbm90ZSByaWdodCBvZiAAIApjcmVhdGUALAVVUkwKADsILT5BcHAAQgZVUkwALw8AFgUAMgdzaGFyZVVSTAB4CkJ1cnN0OgBxCiwAGgoAcxIAJgcAgH8HYnVyc3QKCg&s=napkin)



### User clicks notification link in email or sms
```
IF user has mobile app installed
   Mobile app loads [dustUrl]
ELSE
    App loads in mobile browser from [seedURL]
App loads [dust] from [dustUrl]
IF [dust] not already saved to local.PouchDB
     App saves [dust] to local.PouchDB
IF user logged in
   App syncs local.App.PouchDB <-> StarDust.App.CouchDB
ELSE user not logged in
   Show login fields
```




### [shareUrl] format:
```
https://[seedUrl]/[dustUrl]
```


### Example Dust format
```javascript
{
	id: UUID,
	dts: DateTime,
	node: "zi",
	sector: "creation",
	to: {
		id: UUID,
		name: "Rick James",
		contactVia: "rjames@gmail.com"
	},
	from: {
	    id: UUID,
	    name: "Dave Chappell",
	    contactVia: "dchap@gmail.com"
	},
	parent: dust.UUID,
	message: "Cocaine is a hell of a drug.",
	video: "http://filepicker.io/34jscnas3"
}
```

