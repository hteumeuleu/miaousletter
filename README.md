Miaousletter
============

Voici l'intégration d'un e-mail responsive pour mon atelier à Sud Web le 18 mai 2013. Cet e-mail a été testé via [EmailOnAcid](http://www.emailonacid.com) et avec [CampaignMonitor](http://www.campaignmonitor.com). L'affichage des deux encarts d'articles n'est pas correct sur Lotus Notes 6.5 et 7. 


Bonnes pratiques
----------------

L'intégration de cet e-mail respecte les règles suivantes :

*	Utilisation du Doctype HTML5 (mais testé aussi avec Doctype XHTML, et sans Doctype) (cf [Which doctype should I use in HTML email?](http://www.campaignmonitor.com/blog/post/3317/correct-doctype-to-use-in-html-email/))
*	Ajout d'une ligne de 1000 espaces dans le `<head>` pour forcer le chargement complet sur iOS (cf [Two Ways to Ensure that Your Entire Email Is Rendered by Default in the iPhone & iPad](http://www.emailonacid.com/blog/details/C13/ensure_that_your_entire_email_is_rendered_by_default_in_the_iphone_ipad))
*	Image de fond avec un span (cf [Background Colors in HTML Emails](http://www.emailonacid.com/blog/details/C13/background_colors_in_html_emails)
*	Centrage des tableaux avec un `align="center" style="margin:0 auto;"` sur les balises `<table>` (pour surcharger les styles du webmail d'Orange)
*	Centrage vertical dans une cellule `style="vertical-align:middle;"` sur les balises `<td>` (pour surcharger les styles du webmail d'Orange)
*	Écriture des codes couleurs en hexa sur six caractères (cf [The Best Way to Code Background Colors for HTML Email](https://litmus.com/blog/background-colors-html-email))
*	Style des textes alternatifs (cf [The Ultimate Guide to Styled ALT Text in Email](https://litmus.com/blog/the-ultimate-guide-to-styled-alt-text-in-email))
* 	Utilisation de tableaux flottants pour adapter les blocs en responsive (cf [How does Mailbox app render responsive HTML emails?](http://emailwizardry.nightjar.com.au/2013/04/16/how-does-mailbox-app-render-responsive-html-emails/))
* 	Affichage d'un lien uniquement sur la version mobile (cf [How to display email content in mobile clients only](http://www.campaignmonitor.com/blog/post/3948/hiding-content-in-both-desktop-and-web-email-clients))
*	Privilégie l'utilisation de plusieurs tableaux à la queue leu-leu pour éviter un bon gros bug de #@&%$ sur Outlook sur des e-mails de plus de 1700px de haut (cf [Spacing Issues in Outlook 2007 and 2010](http://www.emailonacid.com/blog/details/C13/horizontal_spacing_issues_in_outlook_2007_and_2010))
* 	Utilisation de bidouilles dégoutantes pour éviter un autre bon gros bug de sur Outlook à cause des tableaux flottants (cf [3 Ways to Remove Unwanted Gaps Between Tables in Outlook 2007 and 2010](http://www.emailonacid.com/blog/details/C13/removing_unwanted_spacing_or_gaps_between_tables_in_outlook_2007_2010) et [L’intégration d’e-mails responsive](http://www.hteumeuleu.fr/integration-emails-responsive/))
*	Utilisation d'un préfixe propre à l'e-mail pour les noms de classe CSS (ex: `miaouMobile`) pour éviter tout conflit avec des classes héritées de webmails (coucou Orange)
*	Ajout de styles (`.ReadMsgBody` et `.ExternalClass`) pour centrer l'e-mail sous Hotmail (cf [Astuce : Afficher correctement un e-mailing sur Hotmail](http://blog.sarbacane.com/2011/06/09/astuce-afficher-correctement-un-e-mailing-sur-hotmail/))

Ressources
----------

Voici quelques ressources intéressantes sur l'intégration d'e-mail :

* 	[Le blog d'EmailOnAcid](http://www.emailonacid.com/blog)
*	[Le blog de CampaignMonitor](http://www.campaignmonitor.com/blog)
*	[Le blog de Litmus](https://litmus.com/blog/)
*	[Les parts de marché des principaux clients mail, par Litmus](http://emailclientmarketshare.com/)
*	[Guide du support CSS chez CampaignMonitor](http://www.campaignmonitor.com/css/)
*	[Guide du support des media queries chez CampaignMonitor](http://www.campaignmonitor.com/guides/mobile/)
*	[Des guides divers chez MailChimp](http://mailchimp.com/resources/) ([Email Marketing Field Guide](http://mailchimp.com/resources/guides/email-marketing-field-guide/) est plutôt cool)
*	[HTML email](http://www.fivesimplesteps.com/products/html-email), un ebook plutôt sympa vendu 2£

Quelques templates d'e-mails :

*	[Email Boilerplate](http://www.emailology.org/) par EmailOnAcid
*	[HTML Email Boilerplate](http://htmlemailboilerplate.com/)
*	[Email Blueprints](https://github.com/mailchimp/Email-Blueprints) par [MailChimp](http://blog.mailchimp.com/introducing-mailchimps-email-template-reference/)
*	[Des templates gratuits](http://templates.sarbacane.com/) par Sarbacane Software

Merci et #bisoudintegrateur