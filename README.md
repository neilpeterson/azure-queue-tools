# Azure Queue Tools

Simple tools built for loading, returning length, and deleting from and Azure Queue.

## Prerequisites:

Azure Storage account and the following environment variables (replace values):

```
# Azure Storage
export AZURE_STORAGE_ACCT=<storage account name>
export AZURE_QUEUE=<queue name>
export AZURE_QUEUE_KEY=F<storage account key>
```

## Usage

### [Load Azure Queue](https://github.com/neilpeterson/azure-queue-tools/blob/master/azure-queue-load.py)

Modify line 17 to controll how many messages are placed on the queue.

```
message_number = randint(50,100)
```

Load messages:

```
python azure-queue-load.py
```

### [Get Queue Length](https://github.com/neilpeterson/azure-queue-tools/blob/master/azure-queue-count.py)

Continuous loop to return Azure Queue length. This can be useful when wanting to monitor queue length.

```
python azure-queue-count.py
```

### [Delete Queue Messages](https://github.com/neilpeterson/azure-queue-tools/blob/master/azure-queue-delete.py)

Deletes all messages from a queue.

```
python azure-queue-delete.py
```