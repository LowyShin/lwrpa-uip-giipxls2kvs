# xls to giip KVS

Read excel file and put to giip KVS.
If you do, you may see data on your mobile device and use condition of trigger point.

## Preparing

* Download giipAgentUIP
  * See [giipAgentUIP](https://github.com/LowyShin/giipAgentUIP)
* Download this repository
  * `git clone https://github.com/LowyShin/lwrpa-uip-giipXLS2KVS.git`
* Check your giip information
  * Account
  * Customer
  * Service
  * SecretKey
  * Logical Machine

## Setting

* giip script
  * Put to script repository
    ```json
    {
        "Execxaml" : "lwrpa-uip-giipXLS2KVS\\XLS2KVS.xaml",
        "sk" : "<giip service secret key>",
        "lssn" : "<giip logical server serial number>",
        "kvsfactor" : "Factor you want",
        "PathSource" : "xlsx file Directory",
        "FileSource" : "xlsx file Name",
        "SheetSource" : "Sheet Name",
        "GitRepoName" : "lwrpa-uip-giipxls2kvs",
        "GitRepoURL" : "https://github.com/LowyShin/lwrpa-uip-giipxls2kvs.git"
    }
    ```
* Run XLS2KVS.xaml on UiPath Studio.
* See Logical server detail page or KVS log page.
* [Get Last KVS data](https://github.com/LowyShin/giip/wiki/getKVSFactorLast)