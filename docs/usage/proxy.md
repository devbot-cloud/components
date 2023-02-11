## Proxy support

When a proxy is configured in the source-controller Pod through the appropriate environment variables, for example HTTPS_PROXY, NO_PROXY, etc. The source-controller will use the proxy for all Git operations. 

This includes the initial clone and subsequent fetches. 

The proxy is also used for the artifact download from the source-controller to the Kubernetes cluster.