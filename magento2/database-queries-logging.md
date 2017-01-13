# Logging database queries

Enable database query logging add the following to your modules di.xml file. See the source article below for more info.

```
<preference for="Magento\Framework\DB\LoggerInterface" type="Magento\Framework\DB\Logger\File"/>
<type name="Magento\Framework\DB\Logger\File">
    <arguments>
        <argument name="logAllQueries" xsi:type="boolean">true</argument>
        <argument name="debugFile" xsi:type="string">debug/atwix.log</argument>
    </arguments>
</type>
```

[source](https://www.atwix.com/magento-2/database-queries-logging/)
