# AWS Lambda Resources

## References
- https://docs.aws.amazon.com/lambda/index.html
- https://docs.aws.amazon.com/lambda/latest/dg/welcome.html
- AWS Lambda Limits
  +  https://docs.aws.amazon.com/lambda/latest/dg/limits.html


## Background Reading
* [The hidden costs of serverless](https://medium.com/@amiram_26122/the-hidden-costs-of-serverless-6ced7844780b)
* https://rclayton.silvrback.com/serverless-isn-t-effortless
* [How Much Does It Cost To Run A Serverless API on AWS?](https://alestic.com/2016/12/aws-invoice-example/)
  * This article walks through the AWS invoice for charges accrued in November 2016 by the TimerCheck.io API service which runs in the us-east-1 (Northern Virginia) region and uses the following AWS services:
* [Paper: Serverless Computing: Economic and Architectural Impact, ESEC/FSE’17, September 4-8, 2017, Paderborn, Germany](https://www.doc.ic.ac.uk/~rbc/papers/fse-serverless-17.pdf)
  * See: Page-3, Table 1: Comparing hostings price for one hour of operation, assuming 200 ms of runtime, executing every five minutes.
* https://techbeacon.com/economics-serverless-computing-real-world-test
  * "The AWS Simple Monthly Calculator features one relatively common application, showing the cost breakdown for running the entire infrastructure stack for a month. The AWS 3-tier auto-scalable web application, written in Ruby on Rails, can serve 100,000 page views a month. The stack consists of one load balancer, two web servers, two application servers, and a highly available database server. The solution also uses DynamoDB, S3, Route53, and CloudFront and has been estimated to require 120 GB of data transfer each month."
  * "The total cost of running this stack is $894.45 per month, of which EC2 compute accounts for $427.04, and RDS for further $337.88.
    Consider how much could be saved if the IaaS compute were to be replaced by AWS Lambda, with API Gateway providing the HTTP facade. While conservatively assuming it takes 3 seconds on average to serve a page view based on the data from RDS or DynamoDB, we can calculate the total cost of serving 100,000 pages. Even with a generous 1 GB memory allocation and relatively sluggish 3-second processing time, the total cost for AWS Lambda would be a mere $5 (this is ignoring the free tier), and API Gateway would add another $11.15!
  * "...using the serverless stack is not always guaranteed to be a money-saving option. There are certain workloads that require substantial compute resources, which makes the serverless model less cost-effective."
* https://forum.serverless.com/t/optimizing-lambdas-reducing-your-bills/4101
* https://blog.binaris.com/my-wish-list-for-aws-lambda-in-2018/


## Case Studies
* https://aws.amazon.com/lambda/resources/customer-case-studies/
* [15 Case studies of AWS serverless apps in production](https://winterwindsoftware.com/real-world-serverless-case-studies/)
* [From $10K/month to $370/month](https://postlight.com/trackchanges/serving-39-million-requests-for-370-month-or-how-we-reduced-our-hosting-costs-by-two-orders-of)
* [Bustle: 84% Reduction in cost...](https://aws.amazon.com/solutions/case-studies/bustle/)
  * Bustle.com is a news, entertainment, lifestyle, and fashion website catering to women. Bustle also operates Romper.com, a website focused on motherhood. Bustle is based in Brooklyn, NY and is read by 50 million people each month.
  * Bustle has also experienced approximately 84% cost savings by moving to a serverless architecture.
* [Projected 94% savings...](https://aws.amazon.com/solutions/case-studies/financial-engines/)
  * Financial Engines is the largest independent investment advisor in the United States, providing technology-enabled portfolio-management services, financial planning, and investment advice to millions of people nationwide.
  * "By using AWS Lambda instead of Amazon EC2 instances for its IPO workload, Financial Engines is realizing an ongoing cost savings. 'We project 94 percent savings in hard costs, or about $110,000 annually'..."
* [Heavywater: 70% savings...](https://read.acloud.guru/how-going-serverless-helped-us-reduce-costs-by-70-255adb87b093)
  * "Even with most of our EC2 instances sized as t2.micro, our AWS bills kept increasing. In the span of just 4 months, our monthly bill increased from $10K to $30K with over 1,000 EC2 instances running."
  * "By the end of November we had converted 80% of our workflows to Step Functions."
  * "After a $30K invoice in September, our AWS bill for the month of December is projected to be less than $4,000."
* [Coca-Cola, from $13K to $4.5K...per year...](https://dzone.com/articles/serverless-case-study-coca-cola)
  * Ater moving to a serverless framework, adding up the costs for all the features they needed, it came down to $4,490/year. This was calculated for the 30 million requests they were getting at the time. Connor stated at AWS re:invent that the break-even point, where having infrastructure as a service would even begin to make sense would be around 80 million calls per month. That's 3 times what they were expecting to get at the time.
  * As the serverless vending machine die off the cost will decrease to the point where if they have less than 1 million requests per month they will get their cost down by 99%.
* [Freight Exchange...](https://www.computerworld.com.au/article/628577/serverless-architecture-delivers-scale-savings-freight-exchange/)
  * "...the number of transactions each month has increased by a factor of 100. But, with the increasingly reliance on serverless computing, hosting costs have remained about the same. "
  * “If you’re going to sit down and go, ‘Right let’s rewrite our entire application to be serverless’, I would say that’s probably a bad idea,” he said.
  * “Maybe you’ll eventually get rid of the whole thing; maybe you won’t’ ever quite get to that. But it doesn’t matter: You’re all the time chipping away and the core bit is getting smaller and you don’t need the same resources. You’re just gradually getting rid of it, but a chunk at a time.”
* [6 things I’ve learned in my first 6 months using serverless](https://read.acloud.guru/six-months-of-serverless-lessons-learned-f6da86a73526)
  * "We are building slick, real-time SPA apps that use exclusively serverless infrastructure, scale effortlessly and cost 70–90% less"
* [Gartner Report (requires purchase): Case Studies in Using Serverless Technologies to Build Commercial Software Products](https://www.gartner.com/doc/3787775/case-studies-using-serverless-technologies)



## Suggested Books
* https://www.amazon.com/AWS-Lambda-Guide-Serverless-Microservices-ebook/dp/B016JOMAEE/




## Articles
### 2020

### 2019 


### 2018
- https://aws.amazon.com/about-aws/whats-new/2018/11/aws-lambda-now-supports-custom-runtimes-and-layers/




## Serverless Conferences
* https://twitter.com/serverlessconf?lang=en
* 2017
  * https://read.acloud.guru/what-you-missed-at-serverlessconf-nyc-3ab02398ebe6
* 2018
  * https://acloud.guru/series/serverlessconf-sf-2018
  * https://serverless.com/blog/serverlessconf-recap-san-francisco-2018-key-takeaways-future-serverless/
  * https://medium.com/lumigo/takeaways-from-the-serverlessconf-sf-2018-7167838394d5
  * https://www.slideshare.net/TimWagner/serverlessconf-2018-keynote-debunking-serverless-myths
  * https://www.slideshare.net/YochayKiriaty/anti-patterns-and-mistakes-using-serverless-serverlessconf-sf-08-2018


## Other Slideshare decks:
* https://www.slideshare.net/marcyterui/reliability-engineering-for-enterprise-serverless


## Github Awesome Serverless Lists
* https://github.com/pmuens/awesome-serverless

