## Docker image for Selenium Server with Chrome (adapted from lzhang/selenium)

* [selenium](http://docs.seleniumhq.org/)

### Installation

```sh
$ sudo docker pull eperoumal/selenium
```

### Usage

Run the container:

```sh
$ SELENIUM_CONTAINER=$(sudo docker run -p 4444:4444 -d eperoumal/selenium)
```

Selenium server will be available on the host machine at port 4444. Web tests 
will run via headless chrome.

Shutting down the container:

```sh
$ sudo docker kill $SELENIUM_CONTAINER
```