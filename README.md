# Zone Markup Language (ZML)

ZML is an XML-based markup language designed for the specification of physical property, in conjunction with the Zone Protocol.

Every piece of property contained within the Zone Protocol is represented as an NFT (non-fungible token), which is linked to an associated deed file. Deed files are specified in ZML.

## ZML Schema Tree

![Schema Tree](/assets/zml-0-1-tree.png)



## Examples

The following is an example ZML deed file for a primary NFT representing a city.

```
<zone level="1" parent="0x" index="42">
    	
    <ttl>604800</ttl>

    <deed type="lease">
        
        <ownership>
        	
        	<title>
        		<key protocol="ETH"> 0xBB9bc244D798123fDe783fCc1C72d3Bb8C189413 </key>
        		<identity protocol="PGP"> 13C1 6474 6800 8E02 25EE 49EC EE8D 0E2E EC9A 96A8</identity>
        		<weight total="1000">500</weight>
        	</title>

        	<quote>
				<key protocol="ETH"> 0x123e1b4dDfd01e4367E687D0561977522452df3D </key>
        		<identity protocol="PGP"> A999 B749 8D1A 8DC4 73E5 3C92 309F 635D AD1B 5517</identity>
        		<weight total="1000">250</weight>
        	</quote>

        	<quote>
        		<key protocol="ETH"> 0x4f9FB88F1f0D68064C4aa425662653D965925883 </key>
        		<identity protocol="PGP"> A999 B749 8D1A 8DC4 73E5 3C92 309F 635D AD1B 5517</identity>
        		<weight total="1000">250</weight>
        	</quote>

        </ownership>

        <dimensions>
        	<name>Las Orillas</name>

        	<description>Zone Authority of Las Orillas City</description>

        	<boundaries protocol="OpenGIS">
        		<map>https://google.com/maps/lorem-ipsum</map>
        		
        		<point>
        			<number>1</number>
        			<coordinates>123456789, 987654321</coordinates>
        		</point>

        		<point>
        			<number>2</number>
        			<coordinates>4736282939, 123123213</coordinates>
        		</point>

        		<point>
        			<number>3</number>
        			<coordinates>123456789, 342343242</coordinates>
        		</point>

        		<point>
        			<number>4</number>
        			<coordinates>3432432432, 3243241126</coordinates>
        		</point>

        	</boundaries>

        </dimensions>

        <history>
        	<record>
        	<timestamp> 1519612175 </timestamp>

        	<digest> ZML 0.1. published. </digest>
        	</record>
        </history>

    </deed>
</zone>
```


