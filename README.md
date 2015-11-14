# docker-dev-base

Use with Docker https://www.docker.io

This image includes git, curl, python, node-gyp, Node.js v4.2.2, TensorFlow for development use.

Build an image with docker as follow:
```bash
cd docker-dev-base
docker build -t="docker-dev-base" .
```	

Then run that image as follow
```bash
docker run -i -t docker-dev-base
```

Run TensorFlow using the official example as follow:
```bash
$ python

>>> import tensorflow as tf
>>> hello = tf.constant('Hello, TensorFlow!')
>>> sess = tf.Session()
>>> print sess.run(hello)
Hello, TensorFlow!
>>> a = tf.constant(10)
>>> b = tf.constant(32)
>>> print sess.run(a+b)
42
>>>
```
