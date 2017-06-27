# Monitoring: Exercise

## Offense

You are a hacker. You live in eastern hackistan. You have a contract with EvilCorp to take down a site that competes with them. Your mission is to take down WellCo!

The discovery phase of your attack has already been completed. A colleague of yours has identified several HTTP endpoints that seem to have weaknesses:

- `/messages`
- `/clocks`
- `/rockets`
- `/beverages`
- `/maps`
- `/pipes`
- `/bins`
- `/handles`
- `/children`

Your task is to pick one of these endpoints, and attack it with everything you have. Try to take down WellCo:

```
yarn run artillery -- quick -o artillery --duration 60 --rate 10 -n 20 http://<your-oponent>/<your-favorite-endpoint>
```

If and when the WellCo engineer can identify the endpoint you are attacking, they will block it, and your attack will be thwarted.

## Defense

You are a dev ops engineer at WellCo - a company that makes products that work well.

You are on call, supporting an app that has been deployed to production.

Unfortunately, this app has gained the reputation for being "the problem app". And now it's 23:30 on a Friday, and you get an SMS message.

The "problem app" is acting up again. You suspect the site may even be under denial-of-service attack.

But how do you identify the vulnerability? Use your knowledge of Logplex and NewRelic to decide which endpoint is being attacked!  Once you've determined that, try to form a hypothesis as to which resource is being used up by the endpoint by inspecting New Relic and Logplex.

## Turn About is Fair Play

After you have successfully attacked and defended an end-point, switch roles! WellCo should attack EvilCorp.

Pick a different endpoint, and work your way through until you can identify the signature of each attack, using Logplex and NewRelic.

Happy hacking!

## Additional Resources

- [Bruce Schneier: The security mirage](https://www.ted.com/talks/bruce_schneier)
