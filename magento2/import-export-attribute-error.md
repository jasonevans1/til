# Magento 2 Import Export Error message

When running a customer import on Magento 2. If the customer attribute does not exist you will get the following error message.

```
1: Begin data validation
2: This file does not contain any data.
```

You can debug the Magento\ImportExport\Model\Import\AbstractEntity::validateData to determine which attribute is causing the error. 
