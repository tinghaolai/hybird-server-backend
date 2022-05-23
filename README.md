# SPEC

## Language
Golang, framework: gin

## API

### Request checking

header: `api-key`

Different token for each user, stored in tables.

### Trading record

* Paginated index
    * Specific day
    * We don't calculate profit percentage here cuz of paginate, Should be calculate by frontend, init when current_page=1, and calculate profit percentage of each row ever since. 
* Add record

## Tables

* users
    * name, api-token
* trading-records
    * user_id, time, balance