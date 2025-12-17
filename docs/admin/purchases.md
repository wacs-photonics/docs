# Purchases

To pass an order there are few steps:

1. Inform your wish on Discord
2. Get a quote
3. Put it in `in-progress` and ask for validation
4. Send the quote to the admin
5. Sign the delivery sheet and send it to the admin
6. Move the files from `in-progress` to `completed`

Details about each step are listed below.

## 1. Inform your wish

For small equipment (e.g. optomechanics, electronics and laboratory materials, etc.), please place a group order whenever possible to limit the number of deliveries. To keep things organized, you have to:

* Open a thread on Discord and indicate a deadline.
* Create an xls file with the list of materials in the `purchases/wish-list` folder on sDrive.
* Ask your colleagues to fill it if they need something before the dealine.

If you plan to buy a specific single equipment, you can skip this step!

## 2. Get a quote

For a list of materials or a single equipement you have to ask for a quote (if you shop online, once you finish with your basket, do not try to finish the order like you would do for a personnal buy. There is usually a button somewhere at the end of the procedure for quote request, or you can directly contact the sales with an email). 
You need to first check the providers with whom we have an account. This includes the most common ones like Thorlabs, Newport, Edmund Optics, RS Pro, etc. If you are not sure check with the admin office if the company is in the database.

Make sure the following information are provided in the quote:

* **Billing adress**: CNRS 1285, CNRS-SCTD, 2 Rue Jean Zay, TSA 61004, 54519 VANDOEUVRE LES NANCY, France
* **Shipping adress**: INPHYNI, UMR7010 CNRS, Institut de Physique de Nice, 17 rue Julien Lauprêtre, 06200 NICE, France
* **VAT number**: FR40180089013

!!! info "Discount"
    We sometimes have special discount with some companies, make sure it has been applied (if not ask your supervisor). You might need to specify a customer ID.<br>
    - For **Thorlabs**, use the **customer ID 404177** to get a 4% discount (except for specific items like microscope objectives). 

!!! warning
    Note that if your item concerns:<br>
    - a consumable (<10 k€), a quote from a single supplier is enough.<br>
    - an equipement (>10 k€), you need to ask for quotes from at least 3 different providers and justify (few sentences) your choice.<br>
    - a large equipement (>40 k€), a specific public market procedure is required (discuss it with your supervisor!)

!!! note "Credit card payment"
    In specific cases, you are allowed to use the lab's credit card to pay directly online or at a shop (after validation from your supervisor off course :smile:). You have to ask the card to *Iliade*. If you use this card then be sure to **get a bill** from the supplier and send it to *Iliade*. The bill should mention your name, the billing address (or at least **INPHYNI, CNRS UMR 7010**). Note that a card ticket is not enough!


## 3. Put it in `in-progress` and ask for validation

Once you obtain your quote, create a dated folder in `in-progress`, add your quote in the `quotes` subfolder and ask for validation to your supervisor.

## 4. Send the quote to the admin

Once validated, send an email to our admin manager *Iliade* with your supervisor in cc. 

You have to specify the **credit source** and the **NACRE nomenclature** (see `purchases/Referentiel_NACRES-janvier2015.xls` in sDrive). For example most of the optics stuff has code *OA-01*, but you are suppose to check for everything single item. To make this part easier, you can have a look and twick [this](https://github.com/laboGigan/thorlabsBC) excellent Python code written by the S. Gigan's team from LKB lab.

*Iliade* will prepare the order (*bon de commande*) and send it to the suppliers. Add the order in the `orders` subfolder for tracking.

## 5. Sign the delivery sheet and send it to the admin
Once your order is delivered (you should receive an notification from *Rachid*), pick it up at the welcome desk, sign the form, check the items and send the signed delivery sheet to *Iliade*.

If it's an online service (e.g. a software licence) without shipping label, fill the form `purchases/Attestation service fait Inphyni.docx` and give it to the admin.

## 6. Move the files from `in-progress` to `completed`
To finalize the procedure, move the whole dated folder from `in-progress` to `completed` and notify your colleagues on the Discord thread.