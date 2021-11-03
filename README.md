# osticket-stuff
Some simple tips for osticket

osticket is a great ticket management tool. We use it for our costumers and anybody else who wants contact.

## disclaimer
I'm no programmer and i just want to offer some small hints here.

## footer for imprint and data privacy guidelines
In the file /include/client/footer.inc.php add these lines before body-end-tag:
```
<div style = "text-align: right;">
    <ul style = "list-style: none;">
      <li style = "display: inline; margin-right: 20px;"><a href = "#link_to_imprint#">Impressum</a></li>
      <li style = "display: inline; margin-right: 20px;"><a href = "#link_to_data_privacy#">Datenschutz</a></li>
      <li style = "display: inline; margin-right: 20px;"><a href = "#link_to_website#">Website</a></li>
    </ul>
</div>
```  

## API key with no static IP
We deployed our websites (wordpress) in a kubernetes-cluster, so there may be several IPs who want to connect to osticket.
One discussion is there: https://github.com/osTicket/osTicket/issues/3857 and the proposed solution (https://github.com/osTicket/osTicket/pull/3932/files) is fine.
