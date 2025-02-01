---
{"dg-publish":true,"dg-path":"trees/How to - DNS Instructions.md","permalink":"/trees/how-to-dns-instructions/","created":"2024-12-14T14:09:54.808-05:00","updated":"2025-01-31T23:05:30.623-05:00"}
---

#topic/web #type/how-to|

# Purchase and Update Nameservers for a New Domain 

## Context

I had the idea for this website late one night when I couldn’t sleep and I was reading about technical writing (for fun), then saw this newsletter in my inbox: [People are looking for me](https://open.substack.com/pub/brassringdaily/p/people-are-looking-for-you). I have PDFs and doc files but not a portfolio that truly represents who I am and what I can do.

It took some time to remember the process of setting up a domain, even though I’ve done it at least 20 times since 1998. DreamHost did a major redesign at some point and I switched servers to A Small Orange, which changed the steps dramatically, but otherwise the steps haven’t changed that much since my first domain registration. Yet it stumps me every time – I wouldn’t expect to have to go to “Manage Registrations” to buy a new domain. I always expect that screen to include the registrations I already have.

This is why I started writing documentation at work in the first place – I was in a troubleshooting position and would have to figure out (for a second time) how to resolve issues I’d seen before. I started writing them down as reference and improved my processing time; the next time a ticket like that came in, my guide told me exactly what to do.

## Gather

You’ll need the following information to complete the below steps:

- Nameserver information for hosting service (I have mine memorized)
- Credit card (DreamHost doesn’t let you use PayPal for the initial purchase of a new domain name)

## Instructions

**Purchase Domain with DreamHost**

1. Login to DreamHost at [https://panel.dreamhost.com](https://panel.dreamhost.com/)
2. Navigate to **Domain Names > Manage Registrations**
3. Search for the domain name you’d like to procure and choose an extension. Follow the prompts to purchase. You may have to wait a few moments for the new domain to show up in your account.

**Update Nameservers to Hosting Service**

4. Navigate to **Websites > Manage Websites**
5. Locate the domain you purchased and select **Manage**
6. Select the **DNS** tab to access Nameserver information
7. Under “Nameservers,” select **Change**
8. Select the “**I’ll use my own nameservers**” option. The fields will become editable.
9. Copy/paste the hosting service’s nameservers into the blanks, remove any extra/blank items, then **Save**. The custom nameservers will appear at the top of the page. This change may take a day or two to propagate across the internet.

**Add Domain to Hosting Service**

1. Login to your website’s Control Panel. In this case, mine uses cPanel.
2. Navigate to **Domains > Addon Domains**
3. **New Domain Name**: Put the domain name here
4. **Subdomain**: Use an appropriate subdomain for this site (this is backend info only)
5. **Document Root**: Update to include public_html (e.g., public_html/maxwrites.me)

After the DNS change propagates across the internet you will be able to visit the website. You can begin development in the Document Root path you defined and when the site becomes available, you’ll find the content there.

Installations that rely on URL data should wait until the DNS change is complete so you don’t have to use the subdomain information in config files.

---
Created: 6/9/23