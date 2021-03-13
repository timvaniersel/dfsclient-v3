# DFS CLIENT v3
To work with this library you'll need an account at [DataForSEO](https://app.dataforseo.com/?aff=123417).

This is a fork with updated dependancies of the official DFSClient that can be found [here](https://github.com/jovixv/DFSClient-v3)

## Installation
```
composer require timvaniersel/dataforseo-clientv3
```

## Usage example
Example usage of setting a task for the SERP API

```
use DFSClientV3\DFSClient as DataForSEO;
use DFSClientV3\Models\SerpApi\SettingSerpTasks;

$client = new DataForSEO(YOUR_DATAFORSEO_LOGIN, YOUR_DATAFORSEO_PASSWORD);
$setting_serp_task = new SettingSerpTasks();
$res = $setting_serp_task->setLanguageCode('nl')->setKeyword('keukenmes')->setPriority('normal')->setLocationCode('9050838')->setSe('google')->setSeType('organic')->get();

```

Visit https://docs.dataforseo.com/v3/ for the official documentation
