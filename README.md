*English instructions are provided below.

このリポジトリには、Unity 6000.0.46f1で使用可能なパッケージが含まれています。  
パッケージをプロジェクトにインポートするには、以下の手順を実行してください。

1. Unityエディタを開き、対象のプロジェクトを開きます。
2. メニューから `Assets > Import Package > Custom Package...` を選択します。
3. ダウンロードしたSimpleWireAction.unitypackageを選択します
4. インポートが終わったらScenes / WireSample.unity を開くとサンプルシーンを動かすことができます

以下のURLでサンプルプロジェクトをブラウザでプレイできます。
https://play.unity.com/ja/games/d5f290cd-57cc-48c6-99ea-31d643070a02/simplewireactionwithhinge2d

---

## Project Structure

### 📁 PreFab
- **Connector.prefab**  
　　Wireの部品がなにかに接触した際に生成される終端のオブジェクト  
- **Player.prefab**  
　　プレイヤーキャラクター  
- **WireBase.prefab**  
　　生成されるWireの部品  

### 📁 Scenes
- **WireSample.unity**  
　　Playerを配置、設定したシーン  

### 📁 Scripts
- **DestroyHinge.cs**  
　　マウスのホールドをやめた際にHingeJoint2Dを削除するスクリプト  
- **DestroyMyself.cs**  
　　Wireの部品やConnectorが落下した際に一定の高さで自身を削除するスクリプト  
- **GrowWire.cs**  
　　PlayerがWireの部品を生成するスクリプト  
- **LaunchWire.cs**  
　　Wireの部品が新たな部品を生成するスクリプト



This repository contains a Unity package compatible with Unity 6000.0.46f1.  
To import the package into your project, follow these steps:

1. Open the Unity Editor and load your target project.
2. From the menu, select `Assets > Import Package > Custom Package...`
3. Choose the downloaded `SimpleWireAction.unitypackage`
4. Once the import is complete, open `Scenes/WireSample.unity` to run the sample scene.

---

## Project Structure

### 📁 PreFab
- **Connector.prefab**  
　　A terminal object that is generated when a wire part comes into contact with something  
- **Player.prefab**  
　　The player character  
- **WireBase.prefab**  
　　A base unit used to generate wire segments  

### 📁 Scenes
- **WireSample.unity**  
　　A sample scene with the Player object placed and configured  

### 📁 Scripts
- **DestroyHinge.cs**  
　　Script that removes the HingeJoint2D when the mouse is released  
- **DestroyMyself.cs**  
　　Script that destroys wire parts or connectors when they fall below a certain height  
- **GrowWire.cs**  
　　Script that allows the player to generate wire segments  
- **LaunchWire.cs**  
　　Script that allows a wire segment to spawn the next segment  
