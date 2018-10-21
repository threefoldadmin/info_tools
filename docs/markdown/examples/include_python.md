
## includes test


### only show class part

'''python
!!!include(name="webserver/JSWebServer.py",repo="https://github.com/threefoldtech/jumpscale_lib", part="class JSWe")
'''

!!!include(name="webserver/JSWebServer.py",repo="https://github.com/threefoldtech/jumpscale_lib", part="class JSWe")

## only show a template part

'''python
!!!include(name="webserver/JSWebServer.py",repo="https://github.com/threefoldtech/jumpscale_lib", part="TEMPLATE")
'''

!!!include(name="webserver/JSWebServer.py",repo="https://github.com/threefoldtech/jumpscale_lib", part="TEMPLATE")

## very specific start & end

'''python
!!!include(name="webserver/JSWebServer.py",repo="https://github.com/threefoldtech/jumpscale_lib", start="TEMPLATE", end="j.servers.web.latest")
'''

!!!include(name="webserver/JSWebServer.py",repo="https://github.com/threefoldtech/jumpscale_lib", start="TEMPLATE", end="j.servers.web.latest")


### the full file

'''python
!!!include(name="webserver/JSWebServer.py",repo="https://github.com/threefoldtech/jumpscale_lib")
'''

!!!include(name="webserver/JSWebServer.py",repo="https://github.com/threefoldtech/jumpscale_lib")
