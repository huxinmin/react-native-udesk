# @wanmi/react-native-udesk

[![GitHub license](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)
[![npm](https://img.shields.io/badge/npm-1.0.6-green)](https://www.npmjs.com/package/@wanmi/react-native-udesk)

## Getting started

`$ npm install @wanmi/react-native-udesk --save`

### Mostly automatic installation

`$ react-native link @wanmi/react-native-udesk`

## Usage
```js
import ReactNativeUdesk from '@wanmi/react-native-udesk';

// 以下是ReactNativeUdesk可使用的方法

/**
 * 用户信息，用于传入这些用户信息，供客服查看
 */
export interface IUserInfo {
    nickname?: string;
    email?: string;
    phone?: string;
    description?: string;
    domain:string;
    appKey:string;
    appId:string;
    sdkToken:string;  //是客户的唯一标识，用来识别身份，可以传userId
}

/**
 * 开始聊天
 * @param {IUserInfo} userInfo 用户信息
 */
export function startChat(userInfo?: IUserInfo): Promise<boolean>
```
