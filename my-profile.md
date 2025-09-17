# 林天友 
## 關於我 
- **Java基礎**
- Android基礎
- C++基礎
> 座右銘：*「我趙活，人醜照活。」*、*「忍一時，風平浪靜，退一步，越想越氣。」*、*「隊友呢？隊友呢？？」*
### **喜歡的[網站](https://www.youtube.com/)**<br />
![趙活本活](https://truth.bahamut.com.tw/s01/202407/forum/73317/0716411046203bb1e662d530b54a4b35.PNG)
> ### 名言：**「平凡如你縱使跌跌撞撞，依然勇於挑戰人生。沒有任何特殊能力，這才叫勇者。」**

|  校名   | 起訖日期  |
|  ----  | ----  |
|  國立彰化師範大學附屬高級工業職業學校 － 資訊科   | 2020/06 ~ 2023/06  |
|  國立高雄科技大學第一校區 － 資訊管理科   | 2023/09 ~ now  |
### - 程式碼
```js
package com.example.va40;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.view.View;

import com.example.va40.databinding.ActivityMainBinding;

public class MainFace extends AppCompatActivity {
    private ActivityMainBinding binding;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        binding = ActivityMainBinding.inflate(getLayoutInflater());
        setContentView(binding.getRoot());

        binding.vapassport.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Intent i = new Intent(MainFace.this, VApassport.class);
                startActivity(i);
            }
        });

        binding.vamail.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Intent i = new Intent(MainFace.this, VAmail.class);
                startActivity(i);
            }
        });
    }
}
```



