# Chat-gpt_streamlit

是基于 chatgpt 的`gpt-3.5-turbo`的 api 的一个小型对话 demo，可以快速部署到streamlit云.
参考于 https://github.com/cwzsquare/chatgpt-streamlit#chatgpt-streamlit

WHY？

国内很多自己很多的朋友想要使用chatgpt，但是由于各种原因，无法使用，之前测试过申请了api_key，但是由于国内的网络问题，无法使用。
在国外的话，朋友又无法访问到国外服务器的网站。
就在搁置的时候，看到了一个streamlit项目，偶然发现streamlit可以部署到云端，切分享之后不受网络影响，于是完善了这个项目并写了这个教程。

解决了：
1. 账号无法注册的问题，现在卖openai账号好像都成生意了，并且甚至很不能注册。
2. 网络问题，现在可以直接部署到streamlit云端，不受网络影响。
3. 不受capacity的限制，可以无限制的使用。

注意：
1. openai的计费问题，自己掌握，不要滥用。
2. 用的模型是gpt-3.5-turbo。
3. 需要提前fork本仓库，然后在app.py中填入自己的api_key，然后部署到streamlit云端。

## 如何使用？
1. 需要填入自己的 api_key ，去 https://platform.openai.com/account/api-keys 申请吧；
2. 部署到streamlit云端，去 https://streamlit.io/cloud 部署吧（建议用github账号登陆）
3. 点击get start
4. 右上角蓝色New app -> From existing app 
5. 选择项目部署，你可以用你fork的项目.
6. Main app file: app.py
7. 点击deploy
8. 最后完成等待即可，完成后分享你的URL，朋友就可以使用了。


## 注意事项
1. 因为使用的streamlit的组件，text_area有一个bug，就是不能在提交后清空，所以每次提交后，需要手动清空。然后才能继续输入下一个问题。暂时没有找到方法解决。
2. 若有朋友有更好的解决方案，欢迎提出。也可以直接pr。或者issue。
3. 如果对大家有帮助的话，欢迎star🌟🌟🌟🌟🌟，fork，issue，pr。