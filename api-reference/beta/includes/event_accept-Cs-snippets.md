
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
	.Accept(comment,sendResponse)
	.Request()
	.PostAsync()

```