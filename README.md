# DataComprassionHW1

用bitset做binary與decimal的轉換會很方便, 最後可能會拿它來做為輸出的工具


10/17   新增資料輸出的解法, 解決越壓縮越大的原因  …
因為cpp一次輸出就要1個byte, 所以如果要輸出一個bit的話, 只能收集8個bit讓他一次輸出, 並且encode完之後的壓縮碼, 不一定要輸出成8bit一個, 因為她並不需要被直接當成圖片來看, 而是應該1個bit1個bit來輸出, 才能達到壓縮的效果
壓縮碼也不需要輸出成.raw, 其實txt也行, 反正他又不是一張圖片

現在就不考慮用bitset輸出了, 可能會用list<bool>收集bits, 然後最後再把他切成8個為一個batch, 一個batch一個batch的輸出
