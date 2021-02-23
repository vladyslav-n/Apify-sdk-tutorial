## Apify-sdk-tutorial
Apify SDK tutorial

## Tutorial II - Apify SDK

*Where and how can you use JQuery with the SDK?*



***

*What is the main difference between Cheerio and JQuery?*

jQuery runs in a browser and attaches directly to the browser's DOM. Cherio parses html from HTTP responses, the same pages you would get in your browser when you first load a URL. The result is the typical $ function, just like in JQuery.

***

*When would you use CheerioCrawler and what are its limitations?*

CheerioCrawler cannot execute JavaScript so it it is not a good fit for pages the content of which depends much on the dynamic elements. Though Cheerio is fast and needs less resources than Puppeteer, so it is a very good choice for the cases where we can avoid difficulties with dynamic content.

***

*What are the main classes for managing requests and when and why would you use one instead of another?*

There are 3 crawler classes available for use in the Apify SDK. BasicCrawler, CheerioCrawler and PuppeteerCrawler.



***

*How can you extract data from a page in Puppeteer without using JQuery?*



***

*What is the default concurrency/parallelism the SDK uses?*


## Tutorial III - Apify Actors & Webhooks

*How do you allocate more CPU for your actor run?*



***

*How can you get the exact time when the actor was started from within the running actor process?*



***

*Which are the default storages an actor run is allocated (connected to)?*



***

*Can you change the memory allocated to a running actor?*



***

*How can you run an actor with Puppeteer in a headful (non-headless) mode?*



***

*Imagine the server/instance the container is running on has a 32 GB, 8-core CPU. What would be the most performant (speed/cost) memory allocation for CheerioCrawler? (Hint: NodeJS processes cannot use user-created threads)*

(Bonus - Docker)

*What is the difference between RUN and CMD Dockerfile commands?*



***

*Does your Dockerfile need to contain a CMD command (assuming we don't want to use ENTRYPOINT which is similar)? If yes or no, why?*



***

*How does the FROM command work and which base images Apify provides?*



## Tutorial IV - Apify CLI & Source Code

*Do you have to rebuild an actor each time the source code is changed?*



***

*What is the difference between pushing your code changes and creating a pull request?*



***

*How does the apify push command work? Is it worth using, in your opinion?*


## Tutorial V - Tasks, Storage, Apify API & Client

*What is the relationship between actor and task?*



***

*What are the differences between default (unnamed) and named storage? Which one would you choose for everyday usage?*



***

*What is the relationship between the Apify API and the Apify client? Are there any significant differences?*



***

*Is it possible to use a request queue for deduplication of product IDs? If yes, how would you do that?*



***

*What is data retention and how does it work for all types of storage (default and named)?*



***

*How do you pass input when running an actor or task via the API?*



## Tutorial VI - Apify Proxy & Bypassing Antiscraping Software

*What types of proxies does the Apify Proxy include? What are the main differences between them?*



***

*Which proxies (proxy groups) can users access with the Apify Proxy trial? How long does this trial last?*



***

*How can you prevent a problem that one of the hardcoded proxy groups that a user is using stops working (a problem with a provider)? What should be the best practices?*



***

*Does it make sense to rotate proxies when you are logged in?*



***

*Construct a proxy URL that will select proxies only from the US (without specific groups).
What do you need to do to rotate proxies (one proxy usually has one IP)? How does this differ for Cheerio Scraper and Puppeteer Scraper?*



***

*Try to set up the Apify Proxy (using any group or auto) in your browser. This is useful for testing how websites behave with proxies from specific countries (although most are from the US). You can try Switchy Omega extension but there are many more. Were you successful?*



***

*Name a few different ways a website can prevent you from scraping it.
Do you know any software companies that develop anti-scraping solutions? Have you ever encountered them on a website?*


## Tutorial VII - Actor Migrations & Maintaining State

*Actors have a Restart on error option in their Settings. Would you use this for your regular actors? Why? When would you use it, and when not?*



***

*Migrations happen randomly, but by setting Restart on error and then throwing an error in the main process, you can force a similar situation. Observe what happens. What changes and what stays the same in a restarted actor run?*



***

*Why don't you usually need to add any special code to handle migrations in normal crawling/scraping? Is there a component that essentially solves this problem for you?*



***

*How can you intercept the migration event? How much time do you need after this takes place and before the actor migrates?*



***

*When would you persist data to a default key-value store and when would you use a named key-value store?*



## Tutorial VIII - Real Project, Communication & QA



Advanced Tutorial - Public Actors


Advanced Tutorial - Proxy country




