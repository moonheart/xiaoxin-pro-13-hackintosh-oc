# add

- 机型/序列号

``` xml
			<key>AdviseWindows</key>
			<false/>
			<key>MLB</key>
			<string>FVF041404GU0000UE</string>
			<key>ROM</key>
			<data>/x//Pw==</data>
			<key>SpoofVendor</key>
			<true/>
			<key>SystemProductName</key>
			<string>MacBookPro15,4</string>
			<key>SystemSerialNumber</key>
			<string>FVFDJ9YNL40Y</string>
			<key>SystemUUID</key>
			<string>8672BE12-75A7-4769-BE23-4034FB23B4E1</string>
```

- AX201 注入

```xml
			<dict>
				<key>BundlePath</key>
				<string>itlwmx.kext</string>
				<key>Comment</key>
				<string>AX201 Wi-Fi</string>
				<key>Enabled</key>
				<true/>
				<key>ExecutablePath</key>
				<string>Contents/MacOS/itlwmx</string>
				<key>MaxKernel</key>
				<string></string>
				<key>MinKernel</key>
				<string></string>
				<key>PlistPath</key>
				<string>Contents/Info.plist</string>
			</dict>
			<dict>
				<key>BundlePath</key>
				<string>IntelBluetoothFirmware.kext</string>
				<key>Comment</key>
				<string>AX201 Bluetooth Firmware</string>
				<key>Enabled</key>
				<true/>
				<key>ExecutablePath</key>
				<string>Contents/MacOS/IntelBluetoothFirmware</string>
				<key>MaxKernel</key>
				<string></string>
				<key>MinKernel</key>
				<string></string>
				<key>PlistPath</key>
				<string>Contents/Info.plist</string>
			</dict>
			<dict>
				<key>BundlePath</key>
				<string>IntelBluetoothInjector.kext</string>
				<key>Comment</key>
				<string>AX201 Bluetooth Switch</string>
				<key>Enabled</key>
				<true/>
				<key>ExecutablePath</key>
				<string></string>
				<key>MaxKernel</key>
				<string></string>
				<key>MinKernel</key>
				<string></string>
				<key>PlistPath</key>
				<string>Contents/Info.plist</string>
			</dict>
```

# remove

- 取消注入网卡

``` xml
            <key>#PciRoot(0x0)/Pci(0x1C,0x0)</key>
            <dict>
                <key>pci-aspm-default</key>
                <data>AgAAAA==</data>
            </dict>
            <key>#PciRoot(0x0)/Pci(0x1C,0x0)/Pci(0x0,0x0)</key>
            <dict>
                <key>pci-aspm-default</key>
                <data>AgEAAA==</data>
            </dict>

```