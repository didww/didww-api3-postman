To do this you need to select a NPA/NXX group by country (US) and region name (New York) as well as by NPA/NXX value (212461). You also need to select a Stock keeping unit (sku_id) which indicates DID number price and one of its available capacity options (usually DID price + 0 channels/2 channels).


> ### Attention
> 
> Requests should be run one-by-one on real environment for real values usage

#### Environment variables

| Name     | Description        |
| -------- | ------------------ |
| `host`   | API host           |
| `apiKey` | Your DIDWW API key |

#### Collection variables

| Name                    | Description                                               |
| ----------------------- | --------------------------------------------------------- |
| `country.id`            | US country id                                             |
| `region.id`             | New York region id                                        |
| `nanpa_prefix.id`       | The id if NPA/NXX prefix group, having NPA: 212, NXX: 461 |
| `stock_keeping_unit.id` | ID of Stock keeping unit with 2 channels included         |