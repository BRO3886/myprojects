---
title: meetings-api
date: 2021-04-12T08:09:14+0000
draft: false
---
<p align="center">
	<h2 align="center">Meetings API (Appointy Task)</h2>
	<h4 align="center">A small, fast meetings api written in Go. Built to Scale.<h4>
  <h5 align="center">Siddhartha Varma, 18BCE0865<h5>
</p>

## Features
- [x]  Built to scale
- [x]  Follows clean architecture
- [x]  Clear separation of concerns

<br>

## Instructions to run

* Pre-requisites:
	-  Golang (1.13+)

* Directions to install

```go
go mod get
```

* Directions to execute

```go
go run .
```


## Note

* I know we only had to use two (2) packages, std net/http and mongo
* I had to use [github.com/joho/godotenv](github.com/joho/godotenv) to protect my mongo URL creds, since I'm using Atlas
* I hope this can be considered