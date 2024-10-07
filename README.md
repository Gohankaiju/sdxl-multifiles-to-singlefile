# SDXL Multi Files to Single File 

Diffusers等によって学習された分割形式のモデルファイルをComfyUIやsd-webuiで使用可能な単一ファイル形式に変換します。

## 注意
このスクリプトの大部分は[sd-scripts](https://github.com/kohya-ss/sd-scripts)のコードを使用させていただいております。オリジナルのコードのライセンスと利用条件を尊重してください。

## 機能
- Diffusers形式のStable Diffusion XLモデルを読み込みます。
- モデルの構造を変換し、単一のSafeTensorsファイルとして保存します。
- コマンドライン引数を使用して、入力モデルと出力先を指定できます。

## 使用方法

```shell
python run.py --model_path <モデルフォルダのパス> [--save_path <保存先パス>]
```
保存パスの指定が無い場合、`/outputs`にモデルファイルが保存されます。

## 動作環境
- CUDA 12.x
- 24GB以上のVRAM
- 必要ライブラリのインポートに関してはsd-scripts様と同様です。[こちら](https://github.com/kohya-ss/sd-scripts)を参照してください。

## ライセンス
Apache-2.0 license