VERSION = 2.16.2
NAME = git

build:
	docker build -t $(NAME) --build-arg VERSION=$(VERSION) .

clean:
	docker rmi $(NAME);

install:
	docker run -it --rm -v /usr/local/:/usr/local/ $(NAME)

dist: build install clean
