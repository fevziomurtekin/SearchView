# SearchView
A beautiful searchview with animations.

# Screens
<table>
  <tr>
    <th>SearchView Animation.</th>
  </tr>
  <tr>
    <td>
      <center><img src="/screen/pincode.gif" width="250" height="350" /></center>
    </td>
  </tr>
</table>
</br>

# Usage

```Gradle
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
  .....

  dependencies {
	        implementation 'com.github.fevziomurtekin:lockscreen:0.1.1'
	  }
	}
  </br> Include layout.`
  ``
  `<com.fevziomurtekin.searchview.SearchView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/search"
        />
        
        
  </br> Include in the activity 
  ```Gradle 
 public class MainActivity extends LookScreen {

    @Override
    protected void onCreate(@Nullable Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        searchView      = new SearchView(getApplicationContext());
        searchView      . setSearchView_hint("Search");
        searchView      . setResult_textSize(14f);
        searchView      . setSearchView_animationTime(250);
        searchView      . setSearchView_textColor(getResources().getColor(R.color.borderColor));
        searchView      . setResult_textSize(14f);
        searchView      . setResult_textColor(getResources().getColor(R.color.borderColor));
    }
}
  ```
  
  # Attributes

  | Attribute | Description |
| --- | --- |
| `title` | Default text, "Enter your password. " |
| `titleSize` | The size in sp of the title text size (by default 15sp) |
| `titleColor` | The color in int of the title text color (R.color.black) |
| `message` | The value in string of the message items (by default "Log in with your password or fingerprint reader.")  |
| `messageSize` |The size in sp of the message text size (by default 14sp) |
| `messageColor` | The color in int of the title text color (R.color.black) |
| `error` | The value in string of the error items (by default "You entered an incorrect password. Please try again.") |
| `errorSize` | The size in sp of the title text size (by default 14sp) |
| `errorColor` | The color in int of the title text color (R.color.red) |
| `intent` | It is for transferring to another class when successfully logged in |
| `pass` | The value in string of the password items (by default "1234") |


## License

    Copyright 2018 Fevzi Ömür Tekin
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
        http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

