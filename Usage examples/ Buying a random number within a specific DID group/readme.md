To do this you need to select a DID Group by country (UK) and city name (London) as well as by DID Group Type (local). You also need to select a Stock keeping unit (sku_id) which indicates DID number price and one of its available capacity options (usually DID price + 0 channels/2 channels).

This is how this functionality looks in DIDWW user panel:

![](https://user-images.githubusercontent.com/120269/143892525-f39554cc-8fa2-4aad-a9f3-6dc4b866e551.png)

> ### Attention
> 
> Requests should be run one-by-one on real environment for real values usage

#### Environment variables

| Name      | Description        |
| --------- | ------------------ |
| `baseUrl` | API host url       |
| `apiKey`  | Your DIDWW API key |

#### Collection variables

| Name                    | Description                                       |
| ----------------------- | ------------------------------------------------- |
| `did_group_type.id`     | Local group type id                               |
| `country.id`            | GB country id                                     |
| `city.id`               | London id                                         |
| `stock_keeping_unit.id` | ID of Stock keeping unit with 2 channels included |