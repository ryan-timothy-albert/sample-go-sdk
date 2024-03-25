<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	"log"
	"petsdk"
)

func main() {
	s := petsdk.New()

	var limit *int = petsdk.Int(21453)

	ctx := context.Background()
	res, err := s.Pets.ListPets(ctx, limit)
	if err != nil {
		log.Fatal(err)
	}
	if res.Pets != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->