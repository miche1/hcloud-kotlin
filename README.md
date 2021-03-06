# hcloud-kotlin
A kotlin api for the hetzner cloud api.

The Hetzner Cloud is a REST-API for managing their Hetzner-Cloud product. 
The API needs a valid token which can be generated on the webinterface from Hetzner:
https://console.hetzner.cloud/

**Getting Started**
```java
    val token : String = "...";
    var hCloud = HCloudApi(token = token);
    //get all created servers
    val servers = hCloud.getServerApi().getServers();
    for(server in servers)
        println(server)

    //get all possible datacenter locations from Hetzner
    val locations = hCloud.getLocationApi().getLocations()
    for(location in locations)
        println(location)
```

**Contributing**

Feel free to open issues on GitHub or fork the repository. If you want support us in any way, you may contact us or you have some ideas for features.. make a pull request. 

Any feedback is welcome!

also see: 
Monitoring project built in Kotlin and the Hetzner Cloud: https://github.com/DDKFM/HCloudMonitoring
