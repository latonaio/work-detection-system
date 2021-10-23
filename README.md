# work-detection-system　　
work-detection-system は、エッジコンピューティング環境において、取得したカメラ映像に対してあらかじめ指定したテンプレート画像および閾値を元にテンプレートマッチングを行い、その結果をUI上に表示するシステムです。  

## 動作環境

* OS: Linux  
* CPU: ARM/AMD/Intel  
* aion-core および 関連リソース  

## work-detection-system のアーキテクチャ   
以下の図はwork-detection-systemのアーキテクチャ図です。  

![work-detection-system](documents/work_detection_system_drowio.png)




## work-detection-system に含まれるリソース

work-detection-system には、以下の マイクロサービス等 のリソースが含まれます。  
・aion-coreおよび関連リソース  
・ui-frontend-for-work-detection  
・ui-backend-for-work-detection  
・control-mitsubishi-plc-r-kube  （※1）  
・control-mitsubishi-plc-w-kube  （※2）  
・template-matching-opencv-for-rtsp  
・summarize-ok-ng-kube  
・import-for-template-matching  

（※1）のマイクロサービスは、次のマイクロサービスに代替されることができます。  
control-jtekt-plc-r-kube, control-yaskawa-robot-r-kube    
（※2）のマイクロサービスは、次のマイクロサービスに代替されることができます。  
control-jtekt-plc-w-kube, control-yaskawa-robot-w    


