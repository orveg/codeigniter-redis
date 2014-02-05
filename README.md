CodeIgniter ElephantIO Liblary
=================

Requirements
------------
1. PHP 5+
2. [CodeIgniter 2.0+](http://codeigniter.com)
3. A [Redis server](http://nodejs.org/)
4. A [socket.io](http://socket.io/)



Documentation
-------------

### Configuration
This library expects a configuration file to function correctly. A template for this file is provided with the library. 


```
$config['socketIOUrl'] = "http://localhost:3030";

```

To use this connection group, you must create a new instance of this library like this:

```
$this->load->library('elephantio/elephantio');

$this->elephantio->init();
$this->elephantio->emit('foo', 'bar');
$this->elephantio->close();

```


License
-------
This library is released under the MIT license.
