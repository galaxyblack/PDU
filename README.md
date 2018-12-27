# PDU:一种点对点的社交网络
Parallel Digital Universe - A Peer-to-Peer Social Network

email: liupeng@tataufo.com

[![GoDoc](https://img.shields.io/badge/godoc-reference-blue.svg)](https://godoc.org/github.com/TATAUFO/PDU)
[![GoReport](https://goreportcard.com/badge/github.com/TATAUFO/PDU)](https://goreportcard.com/report/github.com/TATAUFO/PDU)
[![Travis](https://travis-ci.org/TATAUFO/PDU.svg?branch=master)](https://travis-ci.org/TATAUFO/PDU)
[![License](https://img.shields.io/badge/license-GPL%20v3-blue.svg)](LICENSE)


## Abstract

SNS，即社交网络服务，如Facebook，用户可以在其上创建身份，维护社交关系并进行信息传播，交互。但现有的SNS均依赖于某个第三方的网络服务，而这个第三方（如Facebook）则越来越不被信任。BitTorrent协议，能够实现P2P的信息传播，但其根本目的是提高对于已知内容的传播效率，缺乏在P2P网络下的账号系统，所以无法对未知内容有所判断。即便有数字签名，能够证明每个信息的来源，但是因为缺少第三方验证（如手机号注册），创建账号的成本为零，所以当无用（虚假）的信息会充斥整个网络且无法信息来源进行惩罚。

我们提出一种在纯粹P2P的环境下增加创建成本的方式，并基于这种账户系统，构建完整的P2P社交网络形态。首先我们引入的时间证明，用以证明某个特定行为发生于某时刻之后。新账号的创建必须由多个（通常2个）合法账号签名，同一账号的此类签名操作需满足时间间隔。每个网络的参与者（用户），都在本地以DAG的结构维护所有账号之间的关系拓扑，并随时可以根据自己获知的新消息，对新的账号进行验证增补，同时也可因作恶行为对某些账号及关联账号进行惩罚。

与比特币的共识不同，在PDU中你只相信你所相信的。

## Introduction

现今互联网上的信息传播、交互大多依赖于一个强大可信的第三方中心化服务，如Facebook、Twitter、微信、微博等社交网络服务。但无论有意或无意，第三方服务都存在越权使用用户信息或者造成用户数据泄露的可能。不过在现实情况中，即便明知这种情况已经发生，由于对于三方中心化服务的依赖，很多用户依然不得已选择继续使用发生问题的服务，而非迁移自己的数据。因为对于大多数用户而言，离开某个平台虽然不会损失自己的数据信息，但却失去了在此平台上长期积累的用户关系和自身信用。

我们提出PDU的本意并非完全排除第三方的中心化服务，而是希望能够通过P2P账号系统的实现，能够将用户身份确认及关系拓扑脱离于某个特定平台，用以消除用户对于特定第三方中心化服务的依赖，让用户的身份真正归属于用户。（借此，也能够减轻如facebook、腾讯等对于互联网服务的垄断程度）

我们引入时间证明，并以此为基础订立自然法则。符合自然法则的新建账号才能更广泛的被整个P2P网络所认可，同时每个账号也存在自身的生命周期，在其内的合法信息，才能够获得更为广泛的传播。由此，整个系统的账号数量的增速得到控制， 网络实时的信息总量也可控，同时单个账号也可以根据时间证明来过滤有效账号和时效性高的信息。任何违背自然法则的时间都会作为证据在网络中传播，以利每个用户维护本地的DAG结构的用户拓扑。

时间证明是PDU中用户一切行为成本控制的基础，但因为PDU中没有强制的共识，取而代之的是用户自身的选择，所以完全可能有多个不同的时间证明的存在，或者说多从任何一点，都可能分裂出新的时间线。PDU接收这种情况的存在，就如同平时存在的多个时空，甚至每个时空可以设定不同的时间流速来影响本时空中的行为成本。同时任何用户也可同时存在于自己选择的多个时空当中。	
## Time Proof 


## Account Topology (DAG)
 
## Message (Chain)

## Network

#### Message Spread

#### Account Create

#### PDU Create Step

## Function Node

## Conclusion






















