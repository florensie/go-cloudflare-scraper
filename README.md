Cloudflare Challenge Solver
===========================

A port of (cloudflare-scrape)[https://github.com/Anorov/cloudflare-scrape].

***Not working yet***

Usage
-----

```go
package main

import (
    "github.com/cardigann/cf-challenge-solver"
)


func main() {
	c := http.Client{
		Transport: solver.NewTransport(http.DefaultTransport),
	}

	res, err := c.Get(ts.URL)
	if err != nil {
		log.Fatal(err)
	}

	body, err = ioutil.ReadAll(res.Body)
	res.Body.Close()
	if err != nil {
		log.Fatal(err)
	}
}

