# The Request object

---

# Remember $_GET ?

    !php
    <?php
    echo 'Hello ' . $_GET['name'] . ' !';

.

    !bash
    $ curl http://localhost/labo-web-sf2/web/name.php?name=Adrien
    Hello Adrien !

<br />

---

# Say hello to the Request object

    !php
    use Symfony\Component\HttpFoundation\Request;
    use Symfony\Component\HttpFoundation\Response;

    ...

    public function helloAction(Request $request)
    {
        return new Response('Hello ' . $request->query->get('name') . ' !');
    }

.

    !bash
    $ curl http://localhost/labo-web-sf2/web/name.php?name=Adrien
    Hello Adrien !

---

# $_XXX replacements

* `$request->query` ==> `$_GET`
* `$request->request` ==> `$_POST`
* `$request->server` ==> `$_SERVER`
* `$request->files` ==> `$_FILE`
* `$request->cookies` ==> `$_COOKIE`
* `$request->getSession()` ==> `$_SESSION`
* `$request->attributes` ==> Route parameters and other information (_controller, _route, _route_params, etc)

---

# Cool Request methods

* `$request->getClientIp()` string xxx.xxx.xxx.xxx
* `$request->getMethod()` string (POST, GET, etc)
* `$request->isMethod('POST')` boolean
* `$request->isXmlHttpRequest()` boolean
* `$request->getRequestFormat()` string (html, json, xml, etc)
* `$request->getPreferredLanguage()` string (en_US, fr_FR etc) based on client
