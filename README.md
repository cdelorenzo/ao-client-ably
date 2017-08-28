# ao-client-pubnub
Ably Client Subscriber

## Dependencies
- Requests git
```sh
  sudo yum install git
```

- Requires Node.js to run if installing

```sh
curl --silent --location https://rpm.nodesource.com/setup_6.x | sudo bash -
sudo yum install -y nodejs
```

## setup
    - Pull down code from github

```sh
    git clone https://github.com/cdelorenzo/ao-client-ably.git
    cd ao-client-ably
    npm install
    cp config-default.json config.json # Rename config-default.json to config.json
```

    - update the keys prior to running
    - update the number of connections and ramp time in seconds
```javascript
{
"key":"foo-xxxxx.xxxxx:xxxxxxxxxx",
"environment":"bar-environment",
"connections":"5",
"ramp":"5"
}
```

## Execution

```javascript
    node subscribe.js hostname
```

or use the run


```javascript
    # If you want to execute 4 instances you can use the run helper
    ./run.sh 4
```
