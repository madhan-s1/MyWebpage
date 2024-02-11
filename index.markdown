
<h3>Vnet and subnet</h3>
<table>
    <tr>
        <td>
            <table style="white-space:nowrap;font-size:12px">
                <thead>
			<style>
		          .colored-heading {
				background-colour: red;
				color: DarkBlue;
			}
			</style>
                    <tr>
                        <th class="colored-heading">DC/Region</th>
                        <th class="colored-heading">Subscription</th>
            			<th class="colored-heading">Vnet</th>
                        <th class="colored-heading">CIDR</th>
                        <th class="colored-heading">Master_Subnet</th>
			            <th class="colored-heading">CIDR</th>
                        <th class="colored-heading">Worker_Subnet</th>
                        <th class="colored-heading">CIDR</th>
                    </tr>
                </thead>
		    <style>
		          .colored-data1 {
		            background-colour: black;
		            color: Gunmetal Gray;
			}
		    </style>
                <tbody>
                    {% for member in site.data.vnet_and_subnet %}
                    <tr>
                     
                        <td class="colored-data1">{{ member.DC/Region }}</td>
			            <td class="colored-data1">{{ member.Subscription }}</td>
                        <td class="colored-data1">{{ member.Vnet }}</td>
                        <td class="colored-data1">{{ member.CIDR }}</td>
			            <td class="colored-data1">{{ member.Master_Subnet }}</td>
                        <td class="colored-data1">{{ member.CIDR }}</td>
                        <td class="colored-data1">{{ member.Worker_Subnet }}</td>
                        <td class="colored-data1">{{ member.CIDR }}</td>
                    </tr>
                    {% endfor %}
                </tbody>
            </table>
        </td>
    </tr>
</table>
