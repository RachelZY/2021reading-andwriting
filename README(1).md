# Emotion Recognition based on Intelligent Customer Service Chatbots 

>  Contributed by Zhong Yuan 

## Introduction

人机对话一直是自然语言处理领域内的重要研究方向之一,近年来随着人机交互技术的发展,对话系统正逐渐走向实际应用。其中,智能客服系统受到了很多企业,尤其是大中型企业的广泛关注。智能客服系统旨在解决传统客服模式需要大量人力的现状,在节约人力的同时,使得人工客服在针对特别问题或者特别用户时能够提供更高质量的服务,从而实现“智能客服+人工客服”在服务效率和服务质量两个维度上的整体提升。

新型的智能客服系统在类人能力程度上也被提出了更高的要求。其中,情感能力作为类人能力的重要体现,已经在智能客服系统的各个维度的场景中被实际应用,并且对系统类人能力的提升起到了至关重要的作用。

## Contents

1. 领域综述
2. 领域必读
3. 较新重要
4. 最新可读



## 领域综述

1. Recent advances in deep learning based sentiment analysis

   Sentiment analysis is one of the most popular research areas in natural language processing. It is extremely useful in many applications, such as social media monitoring and e-commerce. Recent application of deep learning based methods has dramatically changed the research strategies and improved the performance of many traditional sentiment analysis tasks, such as sentiment classification and aspect based sentiment analysis. Moreover, it also pushed the boundary of various sentiment analysis task, including sentiment classification of different text granularities and in different application scenarios, implicit sentiment analysis, multimodal sentiment analysis and generation of sentiment-bearing text. In this paper, we give a brief introduction to the recent advance of the deep learning-based methods in these sentiment analysis tasks, including summarizing the approaches and analyzing the dataset. This survey can be well suited for the researchers studying in this field as well as the researchers entering the field.

2. An Emotion Cause Corpus for Chinese Microblogs with Multiple-User Structures

   A notably challenging problem in emotion analysis is recognizing the cause of an emotion. Although there have been a few studies on emotion cause detection, most of them work on news reports or a few of them focus on microblogs using a single-user structure (i.e., all texts in a microblog are written by the same user). In this article, we focus on emotion cause detection for Chinese microblogs using a multiple-user structure (i.e.,texts in a microblog are successively written by several users). First, based on the fact that the causes of an
   emotion of a focused user may be provided by other users in a microblog with the multiple-user structure, we design an emotion cause annotation scheme which can deal with such a complicated case, and then provide an emotion cause corpus using the annotation scheme. Second, based on the analysis of the emotion cause corpus, we formalize two emotion cause detection tasks for microblogs (current-subtweet-based emotion cause detection and original-subtweet-based emotion cause detection). Furthermore, in order to examine the
   difficulty of the two emotion cause detection tasks and the contributions of texts written by different users in a microblog with the multiple-user structure, we choose two popular classification methods (SVM and LSTM) to do emotion cause detection. Our experiments show that the current-subtweet-based emotion cause detection is much more difficult than the original-subtweet-based emotion cause detection, and texts written by different users are very helpful for both emotion cause detection tasks. This study presents a pilot study
   of emotion cause detection which deals with Chinese microblogs using a complicated structure.

3. Joint Learning for Emotion Classification and Emotion Cause Detection  

    We present a neural network-based joint approach for emotion classification and emotion cause detection, which attempts to capture mutual benefits across the two sub-tasks of emotion analysis. Considering that emotion classification and emotion cause detection need different kinds of features (affective and event-based separately), we propose a joint encoder which uses a unified framework to extract features for both sub-tasks and a joint model trainer which simultaneously learns two models for the two sub-tasks separately. Our experiments on Chinese microblogs show that the joint approach is very promising. 

4. Learning Representations from Heterogeneous Network for Sentiment Classification of Product Reviews

   There have been increasing interests in natural language processing to explore effective methods in learning better representations of text for sentiment classification in product reviews. However, most existing methods do not consider subtle interplays among words appeared in review text, authors of reviews and products the reviews are associated with. In this paper, we make use of a heterogeneous network to model the shared polarity in product reviews and learn representations of users, products they commented on and words they used simultaneously.

5. Exploring Overall Opinions for Document Level Sentiment Classification with Structural SVM

   As a fundamental task of sentiment analysis, document level sentiment classification aims to predict user’s overall sentiment (e.g. positive or negative) towards the target in a document. The document usually consists of various opinion sentences towards different aspects with different sentiments. Therefore, the overall opinion towards the whole target should play a more important role in document sentiment prediction. However, most existing methods for the task treat all sentences of the document equally. Thus, they are easy to encounter difficulty when the sentiments of most aspect opinion sentences are not coherent with the overall sentiment.Take the review in Table 1 for example1, it mentions several aspects, and complains about the small size of the memory card and pictures in the dark, however it gives a positive overall rating to the product. The positive overall opinion sentences lead to a positive overall rating though there are many negative opinions towards detailed aspects.


## 领域必读

1. 面向智能客服系统的情感分析技术

   该文以阿里小蜜为例,对智能客服系统中的情感分析技术进行比较全面的介绍,包括情感分析算法模型的原理及其在智能客服系统的多个应用场景中的实际落地使用方式和效果分析。智能客服在解决客户高频业务问题的同时,也需要给客户提供多维度的、具有类人能力的助理、导购、语聊和娱乐等服务,提高客户对智能客服机器人的整体满意度。在此过程中,情感分析技术在机器人类人能力建设中起到了至关重要的作用。该文围绕智能客服系统中人机结合的服务形式,从六个维度总结和介绍了情感分析技术在智能客服系统中的应用场景,包括用户情感检测、用户情感安抚、情感生成式语聊、客服服务质检、会话满意度预估和智能人工入口。

2. 基于句法规则和HowNet的商品评论细粒度观点分析

   利用句法分析对商品评论中评价对象—评价词对的挖掘还存在以下几点不足：一是几乎完全依靠修饰关系进行抽取，抽取到很多无意义的评价对象（非商品属性词），导致产生了大量的噪声，而在后续筛选环节中由于修饰错误的原因很有可能丢失了有用的评价对象或者评价词，不利于评价对象或评价词词典的扩充和修正；二是多数研究只分析句子中的主谓结构，仅抽取到名词性的商品特征作为评价对象，然而，用户评论中商品特征还存在不少通过动词表达的现象，例如，“散热很快”，“散热”的词性标注虽为动词，但其也同样反映了商品的功能，这种“动词＋程度副词＋形容词”的表达句式在评论文本中经常出现，但无法通过主谓结构进行抽取；三是多数观点分析的研究仅基于正面和负面的粗极性分类，难以从整体上解释已购买用户群体对商品属性的偏好程度，因此其他用户无法深入了解商品口碑，商家也无法对比自身产品和竞争对手家的差异，而这却是细粒度观点分析的重要价值。

3. 基于语义规则与RNN模型的在线评论情感分类研究

   电子商务的不断优化使网络购物成为一种重要的消费方式，越来越多的消费者通过点评网站对商品进行评价。但互联网中的商品评论信息内容并不规范且夹杂大量垃圾信息，需借助技术手段对评论信息进行情感分析。因此，如何准确、高效地对评论文本进行情感分析处理，识别出消费者的情感倾向与偏好，成为自然语言处理的重要研究内容之一。

4. 面向商品评论的二元情感认知模型

   电子商务交易规模的不断扩大使得网络商品评论的数量迅速膨胀。海量的商品评论已经超出了人工收集和处理的能力，因此需要计算机自动从大规模评论文本中全面、精炼地筛选出有价值的信息。

5. Cascading Multiway Attention for Document-level Sentiment Classification

   Document-level sentiment classification aims to assign the user reviews a sentiment polarity. Previous methods either just utilized the document content without consideration of user and product information,or did not comprehensively consider what roles the three kinds of information play in text modeling. 

6. ICON: Interactive Conversational Memory Network for Multimodal Emotion Detection

   Emotion recognition in conversations is crucial for building empathetic machines. Current work in this domain do not explicitly consider the inter-personal influences that thrive in the emotional dynamics of dialogues. 

7. A Lexicon-Based Supervised Attention Model for Neural Sentiment Analysis

   Attention mechanisms have been leveraged for sentiment classification tasks because not all words have the same importance. However, most existing attention models did not take full advantage of sentiment lexicons, which provide rich sentiment information and play a critical role in sentiment analysis. 

8. Improving Review Representations with User Attention and Product Attention for Sentiment Classification

   Neural network methods have achieved great success in reviews sentiment classification. Recently, some works achieved improvement by incorporating user and product information to generate a review representation.However,in reviews,we observe that some words or sentences show strong user’s preference,and some others tend to indicate product’s characteristic. The two kinds of information play different roles in determining the sentiment label of a review. Therefore, it is not reasonable to encode user and product information together into one representation.


## 较新重要

1. Emotional Chatting Machine: Emotional Conversation Generation with Internal and External Memory

   There are several challenges in addressing the emotion factor in large-scale conversation generation. First,high-quality emotion-labeled data are difficult to obtain in a large-scale corpus,as emotion annotation is a fairly subjective task and emotion classification is also challenging. Second,it is difficult to consider emotions in a natural and coherent way because we need to balance grammaticality and expressions of emotions. Last,simply embedding emotion information in existing neural models, as shown in our experiments, cannot produce desirable emotional responses but just hard-to-perceive general expressions (which contain only common words that are quite implicit or ambiguous about emotions, and amount to 73.7% of all emotional responses in our dataset).

2. An Efficient Sentiment Analysis Approach for Product Review using Turney Algorithm

   Sentiment analysis can be done by means of Classification and its most important tasks are text categorization,tone recognition,image classification etc. Mostly the extant methods of supervised classification are based on traditional statistics,which can provide ideal results. The main aim is to in crease the accuracy and to report the manufacturer about the negatives of the product. he major problem is categorization of sentiment polarity,which is the problem of sentiment analysis. There are two levels of categorization and they are Review-level Categorization and Sentence-level Categorization. Categorization of review-level becomes arduous when we attempt to classify the reviews respect with their specific rating related to star-scaled. Second,Review-level Categorization has a drawback in Implicit-level sentiment analysis.

3. Dialogue RNN: An Attentive RNN for Emotion Detection in Conversations

   Emotion detection in conversations is a necessary step for a number of applications, including opinion mining over chat history, social media threads, debates, argumentation mining,understanding consumer feedback in live conversations, and so on. Currently systems do not treat the parties in the conversation individually by adapting to the speaker of each utterance.

4. 3D Visualization of Sentiment Measures and Sentiment Classification using Combined Classifier for Customer Product Reviews

   The Internet has wide reachability making many users to buy the products online using e-commerce websites. Usually, users provide their opinions, comments, and reviews about the products in social media, e-commerce websites, blogs, etc. The product review comments provided by the customers have rich information about the usage of the products they bought and their sentiments towards those products.

5. EmotionLines: An Emotion Corpus of Multi-Party Conversations

   Feeling emotion is a critical characteristic to distinguish people from machines. Among all the multi-modal resources for emotion detection, textual datasets are those containing the least additional information in addition to semantics, and hence are adopted widely for testing the developed systems. However, most of the textual emotional datasets consist of emotion labels of only individual words, sentences or documents, which makes it challenging to discuss the contextual flow of emotions.

6. 基于神经主题模型的对话情感分析

   不同于日常生活中的闲聊，客服场景下的对话总是围绕着某些明确的主题展开，例如客户对商品的咨询，对于快递或者商品问题的投诉，等等。对话中句子的情感倾向依赖于整段对话的背景，同一个句子在不同主题的对话中可能有不同的情感倾向，论文主要研究面向客服对话文本的情感分析，旨在对一段对话中的每句话进行情感分类。对话情感分析旨在识别出一段对话中每个句子的情感倾向，其在电商客服数据分析中发挥着关键作用。不同于对单个句子的情感分析，对话中句子的情感倾向依赖于其在对话中的上下文。建立在多任务学习的框架下，该文提出了一个新颖的方法，同时推测一段对话的主题分布和每个句子的情感倾向。对话的主题分布，作为一种全局信息，被嵌入到每个词以及句子的表示中。通过这种方法，每个词和句子被赋予了在特定对话主题下的含义。

7. 基于文本和用户信息的在线评论质量检测

   随着互联网的迅速发展，越来越多的用户评论出现在社交网站上。面对迅速增长的评论数据，如何为阅读评论的消费者提供准确、真实的高质量评论就显得尤为重要。评论质量检测旨在判断在线评论的质量，在传统的研究中，文本信息通常独立地被用于预测评论质量。但是在社交媒体上，每个文本之间不是独立的，而是可以通过发表文本的作者与其他文本相关联，即同一个用户或相近的用户发表的评论质量具有一定的相似性。因此，为了更好的构建文本的表示和研究文本之间基于用户的关联，该文基于神经网络模型分别构建用户和文本的表示，同时，为了放大用户信息的作用，论文进一步将基于注意力机制的用户信息融合到文本中，从而提高文本评论质量检测的效果。

8. 基于自联想记忆与卷积神经网络的跨语言情感分类

   情感分类属于较为典型的二分类问题，即给含有情感色彩的文档一个态度偏向，支持或者反对。西方语言对情感分类研究起步较早，具有丰富的情感词典语料等资源，而中文情感资源相对匮乏。研究跨语言情感分类不仅是为了消除语言之间的应用屏障，还可以将资源丰富型语言的研究资源应用到资源匮乏型语言中去，帮助其他语言发展，跨越语言之间的鸿沟。论文提出一种以商品评论为对象的基于语义融合的跨语言情感分类算法并且结合自联想记忆模型。自联想记忆模型可以减小资源不均衡对分类精度带来的影响，适用于跨语言情感分类任务。

## 最新可读
1. 基于对话结构和联合学习的情感和意图分类

   在社交媒体中存在大量的对话文本，而在这些对话中，说话人的情感和意图通常是相关的。不仅如此，对话的整体结构也会影响对话的情感和意图，因此，需要对对话中的情感和意图进行联合学习。在论文的研究中，将同时考虑各个角色的对话意图和情感，并结合整轮对话考虑两个不同角色之间的情感和意图影响。具体来说，论文基于神经网络模型构建对话文本信息，使用联合学习的网络结构学习意图和情感的内在关系。同时，论文将注意力机制引入一整轮对话之中，目的在于更好地学习对话中上下文的相互影响。

2. 客户来电意图识别研究

​         捕捉客户来电意图信息，开展客户来电意图识别研究具有重要意义。现有的客户来电意图识别大       都是采用人工分析方法，尚没有采用机器学习、深度学习模型识别客户来电意图的研究。为降低人工分析代价，提高客户来电意图识别结果，该文分别从基于传统机器学习模型、基于单／多深度学习模型、基于BERT和深度学习模型组合三个方面，进行客户来电意图识别研究。在移动客服领域客户来电数据上的实验结果显示，F1 值最高达到86.3%，说明该文提出的客户来电意图识别方法是有效的，能够有效帮助移动客服人员进行客户来电意图识别分析。

3.基于用户与产品信息和图卷积网络的情感分类研究

在线评论的情感分类，是评论文本数据挖掘方面的一个重要任务，其主要目的是识别主观文本情感。随着在线评论的数量不断增加，评论内容更是复杂多样，想要通过人工判别的方法去一一分析每一条评论的情感几乎是不可能的，在这个大数据时代，迫切地需要一种自动判别的方法来实现在线评论的情感分类，从而高效地帮助消费者和商家在海量评论文本中获取有价值的信息

4.基于Transformer模型的商品评论情感分析

从用户在互联网上发表的评论信息中挖掘其潜在的商业价值是十分困难的，因为评论信息数量过于庞大，使用人工方式对海量评论信息进行挖掘是不切实际的。文本情感分析技术可以帮助论文从海量数据中挖掘有价值的信息，有效提高效率。





