# mysportsfeeds-go
Go library to use MySportsFeeds API

## Example Use

```
import (
    "context"

    msf "github.com/MySportsFeeds/mysportsfeeds-go"
)

ctx := context.Context
authorization := "Basic asfafasdfasdfasdfasasdfsadfasdfsd"
config := msf.NewConfig(authorization)
client := msf.NewService(config)
options := client.NewSeasonalGamesOptions()
games, statusCode, err := client.SeasonalGames(ctx, options)
```
