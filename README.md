# lightning1

<aura:component implements="flexipage:availableForAllPageTypes,flexipage:availableForRecordHome,force:hasRecordId" access="global" >
	
    <aura:attribute name="buttonLabel" type="string" default="search"/>
    <lightning:layout horizontalAlign="center">
        <lightning:layoutItem padding="around-medium">
        <lightning:select name="selectItem" aura:id="carType" label="AllTypes" variant="label-hidden" value="">
            search your car
            <option value="">Alltypes</option>
            <option value="">SportsCar</option> 
            <option value="">LuxuryCar</option>
            </lightning:select>
        </lightning:layoutItem>
        
        
       <lightning:layoutItem padding="around-medium">
         <lightning:button label="{!v.buttonLabel}" variant="brand" />
         <lightning:button label="new" variant="neutral"/>
       </lightning:layoutItem>
    </lightning:layout>
</aura:component>
