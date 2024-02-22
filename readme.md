# NodeMailer provider - work in progress

Along with Nodemailer npm package use this to avoid paid services like Sendgrid, etc...

## Input:

1. Function callback which returns an array of object consisting of the following
   1. nodemailer config
   2. type (default "no-reply")
2. database config
   1. type (mysql)
   2. table or schema (default: 'emailer')

### Configuration

#### Database schema or structure

##### Mongo
1. sender email
2. type (default "no-reply")
3. config STRING (nodemailer config stringified JSON)
4. sent_count
5. limit
6. time_limit (String) time string in miliseconds

###### Mysql
1. sender email
2. type (default "no-reply")
3. config STRING (nodemailer config stringified JSON)
4. sent_count
5. limit
6. time_limit (String) time string in miliseconds
