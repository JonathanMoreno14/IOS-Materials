# Installing Cocoapods

- Go to your **terminal** and type the following:

```
sudo gem install cocoapods
```
- Then go to your Xcode project folder:

```
pod init

pod install
```
- You should see the following on your terminal:

> [!] Please close any current Xcode sessions and use `appname.xcworkspace` for this project from now on.
Sending stats
Pod installation complete! There are 0 dependencies from the Podfile and 0 total pods installed.

> [!] The Podfile does not contain any dependencies.

> [!] Automatically assigning platform `ios` with version `11.4` on target `appname` because no platform was specified. Please specify a platform for this target in your Podfile. See `https://guides.cocoapods.org/syntax/podfile.html#platform`.

- The Cocoa Pods have been installed on your project

- Next you open **xcworkspace** file  

<img width="104" alt="screen shot 2018-07-27 at 2 06 07 pm" src="https://user-images.githubusercontent.com/11635523/43342006-e90a41c6-91a6-11e8-84e5-c9731cd044cc.png">

- Open your **Podfile**:

<img width="1399" alt="screen shot 2018-07-27 at 2 07 28 pm" src="https://user-images.githubusercontent.com/11635523/43342044-0467f1e8-91a7-11e8-816c-101df8168265.png">



- Your **Podfile** should look like this:

```ruby

# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'ConsumingAPI' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for ConsumingAPI

end

```

> In this example I used Alamofire and SwiftyJSON

- Add the following *Cocoapods*

```ruby

# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'ConsumingAPI' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for ConsumingAPI
  pod 'Alamofire'
  pod 'SwiftyJSON'

end

```

*For more information about [Alamofire](https://github.com/Alamofire/Alamofire) and [SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON)*

- Next your will install the pods via **terminal**  *make sure to install the podfiles within your project folder*

```
pod install
```
> Analyzing dependencies
Downloading dependencies
Installing Alamofire (4.5.0)
Installing SwiftyJSON (3.1.4)
Generating Pods project
Integrating client project
Sending stats
Pod installation complete! There are 2 dependencies from the Podfile and 2 total pods installed.

> [!] Automatically assigning platform `ios` with version `11.4` on target `ConsumingAPI` because no platform was specified. Please specify a platform for this target in your Podfile. See `https://guides.cocoapods.org/syntax/podfile.html#platform`.

- The Cocoapods have been installed
