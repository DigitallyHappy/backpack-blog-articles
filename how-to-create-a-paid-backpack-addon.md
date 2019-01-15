# How to create a paid Backpack Add-on

Status: WIP (not even first draft)

---

My findings:
- you can host private code in a Github organization for as low as $25/mo (unless you've made the mistake of inviting hundreds of developers, like we have in the Backpack organisation)
- _unlike_ repositories from a personal account, organisation repositories allow you to add Outside Collaborators (unlimited, it seems);
- _just like_ repositories from personal accounts, organisation repositories allow you to add deployment SSH keys;

This means, as an indie hacker who wants to **sell _private_ PHP code**, and distribute it through Composer, you should be able to:
- create a Github organisation for your endeavour, and include as many as 4 other people in the smallest pricing tier ($25/mo);
- create a _private_ repository for the package you intend to sell;
- put that package on Packagist.org (_while_ it's public, or _if_ it's public), so that people can install it using composer; alternatively, you could host a [Satis](https://github.com/composer/satis); or use [Private Packagist](https://packagist.com/pricing), but that one is $49/mo for the lowest tier (3 users); alternatively, the Private Packagist vendor add-on should be OK for most developers (1 EUR/customer/month);

This also means, as an indie hacker who wants to **sell _public_ PHP code**, and distribute it through Composer, you should be able to:
- create a free Github organisation for your endeavour, and include as many people as you want, as collaborators or members;
- create a _public_ repository for the package you intend to sell;
- RESTRICT from putting that package on Packagist.org, so that people cannot install it using composer; 
- to allow people to install your package through composer, you could host a [Satis](https://github.com/composer/satis) or use [Private Packagist](https://packagist.com/pricing), for $49/mo for the lowest tier (3 users) or the Private Packagist vendor add-on (1 EUR/paid customer/month);

---

In order to have a clear and simple way for developers to create Backpack add-ons, and monetize them, I intend to prototype the solutions above, and answer these questions:
- [ ] Q1. Can you make a _private_ repository _public_, add it to Packagist.org, then make it _private_?
- [ ] Q2. How difficult is it to use Private Packagist to host a private repository? For the developer.
- [ ] Q3. How difficult is it to install a private repository from Private Packagist? For the customer.
- [ ] Q4. How difficult is it to host your own Satis? For the developer.
- [ ] Q5. How difficult is it to install a private repository from Private Packagist? For the customer.
- [ ] Q5. What's the easiest way for a developer to create a paid Backpack add-on, then monetize it, considering the answers to the above?
- [ ] Q6. Can you monetize a _public_ repository, but restrict installs? How?
- [ ] Q7. For _private_ repositories, can you have free trials?
- [ ] Q8. Can outside collaborators submit and reply to Github Issues?
- [ ] Q9. Can outside collaborators submit Github PRs?
- [ ] Q10. What's the easiest payment provider a developer can use, to charge money for code? Without having to incorporate, without having to send invoices. PayPal perhaps?
- [ ] Q11. What's the correct license for paid packages? A Creative Commons variant maybe?
