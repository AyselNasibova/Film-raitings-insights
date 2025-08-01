```python



import pandas as pd
from google.colab import drive
drive.mount('/content/drive')


file_path = '/content/drive/MyDrive/imdb_top_1000.csv'
df = pd.read_csv(file_path)
df.head()



```

    Drive already mounted at /content/drive; to attempt to forcibly remount, call drive.mount("/content/drive", force_remount=True).






  <div id="df-b1f125f8-abba-498f-9e1c-819d7c9de554" class="colab-df-container">
    <div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Poster_Link</th>
      <th>Series_Title</th>
      <th>Released_Year</th>
      <th>Certificate</th>
      <th>Runtime</th>
      <th>Genre</th>
      <th>IMDB_Rating</th>
      <th>Overview</th>
      <th>Meta_score</th>
      <th>Director</th>
      <th>Star1</th>
      <th>Star2</th>
      <th>Star3</th>
      <th>Star4</th>
      <th>No_of_Votes</th>
      <th>Gross</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>https://m.media-amazon.com/images/M/MV5BMDFkYT...</td>
      <td>The Shawshank Redemption</td>
      <td>1994</td>
      <td>A</td>
      <td>142 min</td>
      <td>Drama</td>
      <td>9.3</td>
      <td>Two imprisoned men bond over a number of years...</td>
      <td>80.0</td>
      <td>Frank Darabont</td>
      <td>Tim Robbins</td>
      <td>Morgan Freeman</td>
      <td>Bob Gunton</td>
      <td>William Sadler</td>
      <td>2343110</td>
      <td>28,341,469</td>
    </tr>
    <tr>
      <th>1</th>
      <td>https://m.media-amazon.com/images/M/MV5BM2MyNj...</td>
      <td>The Godfather</td>
      <td>1972</td>
      <td>A</td>
      <td>175 min</td>
      <td>Crime, Drama</td>
      <td>9.2</td>
      <td>An organized crime dynasty's aging patriarch t...</td>
      <td>100.0</td>
      <td>Francis Ford Coppola</td>
      <td>Marlon Brando</td>
      <td>Al Pacino</td>
      <td>James Caan</td>
      <td>Diane Keaton</td>
      <td>1620367</td>
      <td>134,966,411</td>
    </tr>
    <tr>
      <th>2</th>
      <td>https://m.media-amazon.com/images/M/MV5BMTMxNT...</td>
      <td>The Dark Knight</td>
      <td>2008</td>
      <td>UA</td>
      <td>152 min</td>
      <td>Action, Crime, Drama</td>
      <td>9.0</td>
      <td>When the menace known as the Joker wreaks havo...</td>
      <td>84.0</td>
      <td>Christopher Nolan</td>
      <td>Christian Bale</td>
      <td>Heath Ledger</td>
      <td>Aaron Eckhart</td>
      <td>Michael Caine</td>
      <td>2303232</td>
      <td>534,858,444</td>
    </tr>
    <tr>
      <th>3</th>
      <td>https://m.media-amazon.com/images/M/MV5BMWMwMG...</td>
      <td>The Godfather: Part II</td>
      <td>1974</td>
      <td>A</td>
      <td>202 min</td>
      <td>Crime, Drama</td>
      <td>9.0</td>
      <td>The early life and career of Vito Corleone in ...</td>
      <td>90.0</td>
      <td>Francis Ford Coppola</td>
      <td>Al Pacino</td>
      <td>Robert De Niro</td>
      <td>Robert Duvall</td>
      <td>Diane Keaton</td>
      <td>1129952</td>
      <td>57,300,000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>https://m.media-amazon.com/images/M/MV5BMWU4N2...</td>
      <td>12 Angry Men</td>
      <td>1957</td>
      <td>U</td>
      <td>96 min</td>
      <td>Crime, Drama</td>
      <td>9.0</td>
      <td>A jury holdout attempts to prevent a miscarria...</td>
      <td>96.0</td>
      <td>Sidney Lumet</td>
      <td>Henry Fonda</td>
      <td>Lee J. Cobb</td>
      <td>Martin Balsam</td>
      <td>John Fiedler</td>
      <td>689845</td>
      <td>4,360,000</td>
    </tr>
  </tbody>
</table>
</div>
    <div class="colab-df-buttons">

  <div class="colab-df-container">
    <button class="colab-df-convert" onclick="convertToInteractive('df-b1f125f8-abba-498f-9e1c-819d7c9de554')"
            title="Convert this dataframe to an interactive table."
            style="display:none;">

  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960">
    <path d="M120-120v-720h720v720H120Zm60-500h600v-160H180v160Zm220 220h160v-160H400v160Zm0 220h160v-160H400v160ZM180-400h160v-160H180v160Zm440 0h160v-160H620v160ZM180-180h160v-160H180v160Zm440 0h160v-160H620v160Z"/>
  </svg>
    </button>

  <style>
    .colab-df-container {
      display:flex;
      gap: 12px;
    }

    .colab-df-convert {
      background-color: #E8F0FE;
      border: none;
      border-radius: 50%;
      cursor: pointer;
      display: none;
      fill: #1967D2;
      height: 32px;
      padding: 0 0 0 0;
      width: 32px;
    }

    .colab-df-convert:hover {
      background-color: #E2EBFA;
      box-shadow: 0px 1px 2px rgba(60, 64, 67, 0.3), 0px 1px 3px 1px rgba(60, 64, 67, 0.15);
      fill: #174EA6;
    }

    .colab-df-buttons div {
      margin-bottom: 4px;
    }

    [theme=dark] .colab-df-convert {
      background-color: #3B4455;
      fill: #D2E3FC;
    }

    [theme=dark] .colab-df-convert:hover {
      background-color: #434B5C;
      box-shadow: 0px 1px 3px 1px rgba(0, 0, 0, 0.15);
      filter: drop-shadow(0px 1px 2px rgba(0, 0, 0, 0.3));
      fill: #FFFFFF;
    }
  </style>

    <script>
      const buttonEl =
        document.querySelector('#df-b1f125f8-abba-498f-9e1c-819d7c9de554 button.colab-df-convert');
      buttonEl.style.display =
        google.colab.kernel.accessAllowed ? 'block' : 'none';

      async function convertToInteractive(key) {
        const element = document.querySelector('#df-b1f125f8-abba-498f-9e1c-819d7c9de554');
        const dataTable =
          await google.colab.kernel.invokeFunction('convertToInteractive',
                                                    [key], {});
        if (!dataTable) return;

        const docLinkHtml = 'Like what you see? Visit the ' +
          '<a target="_blank" href=https://colab.research.google.com/notebooks/data_table.ipynb>data table notebook</a>'
          + ' to learn more about interactive tables.';
        element.innerHTML = '';
        dataTable['output_type'] = 'display_data';
        await google.colab.output.renderOutput(dataTable, element);
        const docLink = document.createElement('div');
        docLink.innerHTML = docLinkHtml;
        element.appendChild(docLink);
      }
    </script>
  </div>


    <div id="df-c43d0c1e-9d1c-4da0-93b3-65e2efb4bdf6">
      <button class="colab-df-quickchart" onclick="quickchart('df-c43d0c1e-9d1c-4da0-93b3-65e2efb4bdf6')"
                title="Suggest charts"
                style="display:none;">

<svg xmlns="http://www.w3.org/2000/svg" height="24px"viewBox="0 0 24 24"
     width="24px">
    <g>
        <path d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zM9 17H7v-7h2v7zm4 0h-2V7h2v10zm4 0h-2v-4h2v4z"/>
    </g>
</svg>
      </button>

<style>
  .colab-df-quickchart {
      --bg-color: #E8F0FE;
      --fill-color: #1967D2;
      --hover-bg-color: #E2EBFA;
      --hover-fill-color: #174EA6;
      --disabled-fill-color: #AAA;
      --disabled-bg-color: #DDD;
  }

  [theme=dark] .colab-df-quickchart {
      --bg-color: #3B4455;
      --fill-color: #D2E3FC;
      --hover-bg-color: #434B5C;
      --hover-fill-color: #FFFFFF;
      --disabled-bg-color: #3B4455;
      --disabled-fill-color: #666;
  }

  .colab-df-quickchart {
    background-color: var(--bg-color);
    border: none;
    border-radius: 50%;
    cursor: pointer;
    display: none;
    fill: var(--fill-color);
    height: 32px;
    padding: 0;
    width: 32px;
  }

  .colab-df-quickchart:hover {
    background-color: var(--hover-bg-color);
    box-shadow: 0 1px 2px rgba(60, 64, 67, 0.3), 0 1px 3px 1px rgba(60, 64, 67, 0.15);
    fill: var(--button-hover-fill-color);
  }

  .colab-df-quickchart-complete:disabled,
  .colab-df-quickchart-complete:disabled:hover {
    background-color: var(--disabled-bg-color);
    fill: var(--disabled-fill-color);
    box-shadow: none;
  }

  .colab-df-spinner {
    border: 2px solid var(--fill-color);
    border-color: transparent;
    border-bottom-color: var(--fill-color);
    animation:
      spin 1s steps(1) infinite;
  }

  @keyframes spin {
    0% {
      border-color: transparent;
      border-bottom-color: var(--fill-color);
      border-left-color: var(--fill-color);
    }
    20% {
      border-color: transparent;
      border-left-color: var(--fill-color);
      border-top-color: var(--fill-color);
    }
    30% {
      border-color: transparent;
      border-left-color: var(--fill-color);
      border-top-color: var(--fill-color);
      border-right-color: var(--fill-color);
    }
    40% {
      border-color: transparent;
      border-right-color: var(--fill-color);
      border-top-color: var(--fill-color);
    }
    60% {
      border-color: transparent;
      border-right-color: var(--fill-color);
    }
    80% {
      border-color: transparent;
      border-right-color: var(--fill-color);
      border-bottom-color: var(--fill-color);
    }
    90% {
      border-color: transparent;
      border-bottom-color: var(--fill-color);
    }
  }
</style>

      <script>
        async function quickchart(key) {
          const quickchartButtonEl =
            document.querySelector('#' + key + ' button');
          quickchartButtonEl.disabled = true;  // To prevent multiple clicks.
          quickchartButtonEl.classList.add('colab-df-spinner');
          try {
            const charts = await google.colab.kernel.invokeFunction(
                'suggestCharts', [key], {});
          } catch (error) {
            console.error('Error during call to suggestCharts:', error);
          }
          quickchartButtonEl.classList.remove('colab-df-spinner');
          quickchartButtonEl.classList.add('colab-df-quickchart-complete');
        }
        (() => {
          let quickchartButtonEl =
            document.querySelector('#df-c43d0c1e-9d1c-4da0-93b3-65e2efb4bdf6 button');
          quickchartButtonEl.style.display =
            google.colab.kernel.accessAllowed ? 'block' : 'none';
        })();
      </script>
    </div>

    </div>
  </div>




# Məlumatların təmizlənməsi



```python
# 'Poster_Link' sütununu silirik (əgər varsa)
if "Poster_Link" in df.columns:
    df = df.drop("Poster_Link", axis=1)

# 'Not Available' olan illəri çıxardırıq
df = df[df["Released_Year"] != "Not Available"]


# Müddət sütunundakı " min" hissəsini çıxardırıq və ədədə çeviririk
df["Runtime"] = df["Runtime"].astype(str).str.replace(" min", "")
df["Runtime"] = pd.to_numeric(df["Runtime"], errors="coerce")



# Boş sertifikatları "Unknown" ilə əvəz edirik
df["Certificate"] = df["Certificate"].fillna("Unknown")

# Meta skor üçün boşluqları orta dəyərlə əvəz edirik
df["Meta_score"] = df["Meta_score"].fillna(df["Meta_score"].mean())

# Gəlir üçün boşluqları median dəyərlə doldururuq
df["Gross"] = df["Gross"].fillna(df["Gross"].median())

# Əsas sütunlarda boş sətrləri silirik
df = df.dropna(subset=["Released_Year", "Runtime", "IMDB_Rating"])
df["Gross"] = df["Gross"].astype(str).str.replace(",", "", regex=False)
df["Gross"] = pd.to_numeric(df["Gross"], errors="coerce")
df["Gross"] = df["Gross"].astype(int)

```


```python
# Показывать все строки
pd.set_option('display.max_rows', None)

# Показывать все столбцы
pd.set_option('display.max_columns', None)

# Показать весь DataFrame
df
```





  <div id="df-ca33b6c3-969b-4742-b2ec-ea067f6317fe" class="colab-df-container">
    <div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Series_Title</th>
      <th>Released_Year</th>
      <th>Certificate</th>
      <th>Runtime</th>
      <th>Genre</th>
      <th>IMDB_Rating</th>
      <th>Overview</th>
      <th>Meta_score</th>
      <th>Director</th>
      <th>Star1</th>
      <th>Star2</th>
      <th>Star3</th>
      <th>Star4</th>
      <th>No_of_Votes</th>
      <th>Gross</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>The Shawshank Redemption</td>
      <td>1994</td>
      <td>A</td>
      <td>142</td>
      <td>Drama</td>
      <td>9.3</td>
      <td>Two imprisoned men bond over a number of years...</td>
      <td>80.00000</td>
      <td>Frank Darabont</td>
      <td>Tim Robbins</td>
      <td>Morgan Freeman</td>
      <td>Bob Gunton</td>
      <td>William Sadler</td>
      <td>2343110</td>
      <td>28341469</td>
    </tr>
    <tr>
      <th>1</th>
      <td>The Godfather</td>
      <td>1972</td>
      <td>A</td>
      <td>175</td>
      <td>Crime, Drama</td>
      <td>9.2</td>
      <td>An organized crime dynasty's aging patriarch t...</td>
      <td>100.00000</td>
      <td>Francis Ford Coppola</td>
      <td>Marlon Brando</td>
      <td>Al Pacino</td>
      <td>James Caan</td>
      <td>Diane Keaton</td>
      <td>1620367</td>
      <td>134966411</td>
    </tr>
    <tr>
      <th>2</th>
      <td>The Dark Knight</td>
      <td>2008</td>
      <td>UA</td>
      <td>152</td>
      <td>Action, Crime, Drama</td>
      <td>9.0</td>
      <td>When the menace known as the Joker wreaks havo...</td>
      <td>84.00000</td>
      <td>Christopher Nolan</td>
      <td>Christian Bale</td>
      <td>Heath Ledger</td>
      <td>Aaron Eckhart</td>
      <td>Michael Caine</td>
      <td>2303232</td>
      <td>534858444</td>
    </tr>
    <tr>
      <th>3</th>
      <td>The Godfather: Part II</td>
      <td>1974</td>
      <td>A</td>
      <td>202</td>
      <td>Crime, Drama</td>
      <td>9.0</td>
      <td>The early life and career of Vito Corleone in ...</td>
      <td>90.00000</td>
      <td>Francis Ford Coppola</td>
      <td>Al Pacino</td>
      <td>Robert De Niro</td>
      <td>Robert Duvall</td>
      <td>Diane Keaton</td>
      <td>1129952</td>
      <td>57300000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>12 Angry Men</td>
      <td>1957</td>
      <td>U</td>
      <td>96</td>
      <td>Crime, Drama</td>
      <td>9.0</td>
      <td>A jury holdout attempts to prevent a miscarria...</td>
      <td>96.00000</td>
      <td>Sidney Lumet</td>
      <td>Henry Fonda</td>
      <td>Lee J. Cobb</td>
      <td>Martin Balsam</td>
      <td>John Fiedler</td>
      <td>689845</td>
      <td>4360000</td>
    </tr>
    <tr>
      <th>5</th>
      <td>The Lord of the Rings: The Return of the King</td>
      <td>2003</td>
      <td>U</td>
      <td>201</td>
      <td>Action, Adventure, Drama</td>
      <td>8.9</td>
      <td>Gandalf and Aragorn lead the World of Men agai...</td>
      <td>94.00000</td>
      <td>Peter Jackson</td>
      <td>Elijah Wood</td>
      <td>Viggo Mortensen</td>
      <td>Ian McKellen</td>
      <td>Orlando Bloom</td>
      <td>1642758</td>
      <td>377845905</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Pulp Fiction</td>
      <td>1994</td>
      <td>A</td>
      <td>154</td>
      <td>Crime, Drama</td>
      <td>8.9</td>
      <td>The lives of two mob hitmen, a boxer, a gangst...</td>
      <td>94.00000</td>
      <td>Quentin Tarantino</td>
      <td>John Travolta</td>
      <td>Uma Thurman</td>
      <td>Samuel L. Jackson</td>
      <td>Bruce Willis</td>
      <td>1826188</td>
      <td>107928762</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Schindler's List</td>
      <td>1993</td>
      <td>A</td>
      <td>195</td>
      <td>Biography, Drama, History</td>
      <td>8.9</td>
      <td>In German-occupied Poland during World War II,...</td>
      <td>94.00000</td>
      <td>Steven Spielberg</td>
      <td>Liam Neeson</td>
      <td>Ralph Fiennes</td>
      <td>Ben Kingsley</td>
      <td>Caroline Goodall</td>
      <td>1213505</td>
      <td>96898818</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Inception</td>
      <td>2010</td>
      <td>UA</td>
      <td>148</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>8.8</td>
      <td>A thief who steals corporate secrets through t...</td>
      <td>74.00000</td>
      <td>Christopher Nolan</td>
      <td>Leonardo DiCaprio</td>
      <td>Joseph Gordon-Levitt</td>
      <td>Elliot Page</td>
      <td>Ken Watanabe</td>
      <td>2067042</td>
      <td>292576195</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Fight Club</td>
      <td>1999</td>
      <td>A</td>
      <td>139</td>
      <td>Drama</td>
      <td>8.8</td>
      <td>An insomniac office worker and a devil-may-car...</td>
      <td>66.00000</td>
      <td>David Fincher</td>
      <td>Brad Pitt</td>
      <td>Edward Norton</td>
      <td>Meat Loaf</td>
      <td>Zach Grenier</td>
      <td>1854740</td>
      <td>37030102</td>
    </tr>
    <tr>
      <th>10</th>
      <td>The Lord of the Rings: The Fellowship of the Ring</td>
      <td>2001</td>
      <td>U</td>
      <td>178</td>
      <td>Action, Adventure, Drama</td>
      <td>8.8</td>
      <td>A meek Hobbit from the Shire and eight compani...</td>
      <td>92.00000</td>
      <td>Peter Jackson</td>
      <td>Elijah Wood</td>
      <td>Ian McKellen</td>
      <td>Orlando Bloom</td>
      <td>Sean Bean</td>
      <td>1661481</td>
      <td>315544750</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Forrest Gump</td>
      <td>1994</td>
      <td>UA</td>
      <td>142</td>
      <td>Drama, Romance</td>
      <td>8.8</td>
      <td>The presidencies of Kennedy and Johnson, the e...</td>
      <td>82.00000</td>
      <td>Robert Zemeckis</td>
      <td>Tom Hanks</td>
      <td>Robin Wright</td>
      <td>Gary Sinise</td>
      <td>Sally Field</td>
      <td>1809221</td>
      <td>330252182</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Il buono, il brutto, il cattivo</td>
      <td>1966</td>
      <td>A</td>
      <td>161</td>
      <td>Western</td>
      <td>8.8</td>
      <td>A bounty hunting scam joins two men in an unea...</td>
      <td>90.00000</td>
      <td>Sergio Leone</td>
      <td>Clint Eastwood</td>
      <td>Eli Wallach</td>
      <td>Lee Van Cleef</td>
      <td>Aldo Giuffrè</td>
      <td>688390</td>
      <td>6100000</td>
    </tr>
    <tr>
      <th>13</th>
      <td>The Lord of the Rings: The Two Towers</td>
      <td>2002</td>
      <td>UA</td>
      <td>179</td>
      <td>Action, Adventure, Drama</td>
      <td>8.7</td>
      <td>While Frodo and Sam edge closer to Mordor with...</td>
      <td>87.00000</td>
      <td>Peter Jackson</td>
      <td>Elijah Wood</td>
      <td>Ian McKellen</td>
      <td>Viggo Mortensen</td>
      <td>Orlando Bloom</td>
      <td>1485555</td>
      <td>342551365</td>
    </tr>
    <tr>
      <th>14</th>
      <td>The Matrix</td>
      <td>1999</td>
      <td>A</td>
      <td>136</td>
      <td>Action, Sci-Fi</td>
      <td>8.7</td>
      <td>When a beautiful stranger leads computer hacke...</td>
      <td>73.00000</td>
      <td>Lana Wachowski</td>
      <td>Lilly Wachowski</td>
      <td>Keanu Reeves</td>
      <td>Laurence Fishburne</td>
      <td>Carrie-Anne Moss</td>
      <td>1676426</td>
      <td>171479930</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Goodfellas</td>
      <td>1990</td>
      <td>A</td>
      <td>146</td>
      <td>Biography, Crime, Drama</td>
      <td>8.7</td>
      <td>The story of Henry Hill and his life in the mo...</td>
      <td>90.00000</td>
      <td>Martin Scorsese</td>
      <td>Robert De Niro</td>
      <td>Ray Liotta</td>
      <td>Joe Pesci</td>
      <td>Lorraine Bracco</td>
      <td>1020727</td>
      <td>46836394</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Star Wars: Episode V - The Empire Strikes Back</td>
      <td>1980</td>
      <td>UA</td>
      <td>124</td>
      <td>Action, Adventure, Fantasy</td>
      <td>8.7</td>
      <td>After the Rebels are brutally overpowered by t...</td>
      <td>82.00000</td>
      <td>Irvin Kershner</td>
      <td>Mark Hamill</td>
      <td>Harrison Ford</td>
      <td>Carrie Fisher</td>
      <td>Billy Dee Williams</td>
      <td>1159315</td>
      <td>290475067</td>
    </tr>
    <tr>
      <th>17</th>
      <td>One Flew Over the Cuckoo's Nest</td>
      <td>1975</td>
      <td>A</td>
      <td>133</td>
      <td>Drama</td>
      <td>8.7</td>
      <td>A criminal pleads insanity and is admitted to ...</td>
      <td>83.00000</td>
      <td>Milos Forman</td>
      <td>Jack Nicholson</td>
      <td>Louise Fletcher</td>
      <td>Michael Berryman</td>
      <td>Peter Brocco</td>
      <td>918088</td>
      <td>112000000</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Hamilton</td>
      <td>2020</td>
      <td>PG-13</td>
      <td>160</td>
      <td>Biography, Drama, History</td>
      <td>8.6</td>
      <td>The real life of one of America's foremost fou...</td>
      <td>90.00000</td>
      <td>Thomas Kail</td>
      <td>Lin-Manuel Miranda</td>
      <td>Phillipa Soo</td>
      <td>Leslie Odom Jr.</td>
      <td>Renée Elise Goldsberry</td>
      <td>55291</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Gisaengchung</td>
      <td>2019</td>
      <td>A</td>
      <td>132</td>
      <td>Comedy, Drama, Thriller</td>
      <td>8.6</td>
      <td>Greed and class discrimination threaten the ne...</td>
      <td>96.00000</td>
      <td>Bong Joon Ho</td>
      <td>Kang-ho Song</td>
      <td>Lee Sun-kyun</td>
      <td>Cho Yeo-jeong</td>
      <td>Choi Woo-sik</td>
      <td>552778</td>
      <td>53367844</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Soorarai Pottru</td>
      <td>2020</td>
      <td>U</td>
      <td>153</td>
      <td>Drama</td>
      <td>8.6</td>
      <td>Nedumaaran Rajangam "Maara" sets out to make t...</td>
      <td>77.97153</td>
      <td>Sudha Kongara</td>
      <td>Suriya</td>
      <td>Madhavan</td>
      <td>Paresh Rawal</td>
      <td>Aparna Balamurali</td>
      <td>54995</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Interstellar</td>
      <td>2014</td>
      <td>UA</td>
      <td>169</td>
      <td>Adventure, Drama, Sci-Fi</td>
      <td>8.6</td>
      <td>A team of explorers travel through a wormhole ...</td>
      <td>74.00000</td>
      <td>Christopher Nolan</td>
      <td>Matthew McConaughey</td>
      <td>Anne Hathaway</td>
      <td>Jessica Chastain</td>
      <td>Mackenzie Foy</td>
      <td>1512360</td>
      <td>188020017</td>
    </tr>
    <tr>
      <th>22</th>
      <td>Cidade de Deus</td>
      <td>2002</td>
      <td>A</td>
      <td>130</td>
      <td>Crime, Drama</td>
      <td>8.6</td>
      <td>In the slums of Rio, two kids' paths diverge a...</td>
      <td>79.00000</td>
      <td>Fernando Meirelles</td>
      <td>Kátia Lund</td>
      <td>Alexandre Rodrigues</td>
      <td>Leandro Firmino</td>
      <td>Matheus Nachtergaele</td>
      <td>699256</td>
      <td>7563397</td>
    </tr>
    <tr>
      <th>23</th>
      <td>Sen to Chihiro no kamikakushi</td>
      <td>2001</td>
      <td>U</td>
      <td>125</td>
      <td>Animation, Adventure, Family</td>
      <td>8.6</td>
      <td>During her family's move to the suburbs, a sul...</td>
      <td>96.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Daveigh Chase</td>
      <td>Suzanne Pleshette</td>
      <td>Miyu Irino</td>
      <td>Rumi Hiiragi</td>
      <td>651376</td>
      <td>10055859</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Saving Private Ryan</td>
      <td>1998</td>
      <td>R</td>
      <td>169</td>
      <td>Drama, War</td>
      <td>8.6</td>
      <td>Following the Normandy Landings, a group of U....</td>
      <td>91.00000</td>
      <td>Steven Spielberg</td>
      <td>Tom Hanks</td>
      <td>Matt Damon</td>
      <td>Tom Sizemore</td>
      <td>Edward Burns</td>
      <td>1235804</td>
      <td>216540909</td>
    </tr>
    <tr>
      <th>25</th>
      <td>The Green Mile</td>
      <td>1999</td>
      <td>A</td>
      <td>189</td>
      <td>Crime, Drama, Fantasy</td>
      <td>8.6</td>
      <td>The lives of guards on Death Row are affected ...</td>
      <td>61.00000</td>
      <td>Frank Darabont</td>
      <td>Tom Hanks</td>
      <td>Michael Clarke Duncan</td>
      <td>David Morse</td>
      <td>Bonnie Hunt</td>
      <td>1147794</td>
      <td>136801374</td>
    </tr>
    <tr>
      <th>26</th>
      <td>La vita è bella</td>
      <td>1997</td>
      <td>U</td>
      <td>116</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.6</td>
      <td>When an open-minded Jewish librarian and his s...</td>
      <td>59.00000</td>
      <td>Roberto Benigni</td>
      <td>Roberto Benigni</td>
      <td>Nicoletta Braschi</td>
      <td>Giorgio Cantarini</td>
      <td>Giustino Durano</td>
      <td>623629</td>
      <td>57598247</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Se7en</td>
      <td>1995</td>
      <td>A</td>
      <td>127</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.6</td>
      <td>Two detectives, a rookie and a veteran, hunt a...</td>
      <td>65.00000</td>
      <td>David Fincher</td>
      <td>Morgan Freeman</td>
      <td>Brad Pitt</td>
      <td>Kevin Spacey</td>
      <td>Andrew Kevin Walker</td>
      <td>1445096</td>
      <td>100125643</td>
    </tr>
    <tr>
      <th>28</th>
      <td>The Silence of the Lambs</td>
      <td>1991</td>
      <td>A</td>
      <td>118</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.6</td>
      <td>A young F.B.I. cadet must receive the help of ...</td>
      <td>85.00000</td>
      <td>Jonathan Demme</td>
      <td>Jodie Foster</td>
      <td>Anthony Hopkins</td>
      <td>Lawrence A. Bonney</td>
      <td>Kasi Lemmons</td>
      <td>1270197</td>
      <td>130742922</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Star Wars</td>
      <td>1977</td>
      <td>UA</td>
      <td>121</td>
      <td>Action, Adventure, Fantasy</td>
      <td>8.6</td>
      <td>Luke Skywalker joins forces with a Jedi Knight...</td>
      <td>90.00000</td>
      <td>George Lucas</td>
      <td>Mark Hamill</td>
      <td>Harrison Ford</td>
      <td>Carrie Fisher</td>
      <td>Alec Guinness</td>
      <td>1231473</td>
      <td>322740140</td>
    </tr>
    <tr>
      <th>30</th>
      <td>Seppuku</td>
      <td>1962</td>
      <td>Unknown</td>
      <td>133</td>
      <td>Action, Drama, Mystery</td>
      <td>8.6</td>
      <td>When a ronin requesting seppuku at a feudal lo...</td>
      <td>85.00000</td>
      <td>Masaki Kobayashi</td>
      <td>Tatsuya Nakadai</td>
      <td>Akira Ishihama</td>
      <td>Shima Iwashita</td>
      <td>Tetsurô Tanba</td>
      <td>42004</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>31</th>
      <td>Shichinin no samurai</td>
      <td>1954</td>
      <td>U</td>
      <td>207</td>
      <td>Action, Adventure, Drama</td>
      <td>8.6</td>
      <td>A poor village under attack by bandits recruit...</td>
      <td>98.00000</td>
      <td>Akira Kurosawa</td>
      <td>Toshirô Mifune</td>
      <td>Takashi Shimura</td>
      <td>Keiko Tsushima</td>
      <td>Yukiko Shimazaki</td>
      <td>315744</td>
      <td>269061</td>
    </tr>
    <tr>
      <th>32</th>
      <td>It's a Wonderful Life</td>
      <td>1946</td>
      <td>PG</td>
      <td>130</td>
      <td>Drama, Family, Fantasy</td>
      <td>8.6</td>
      <td>An angel is sent from Heaven to help a despera...</td>
      <td>89.00000</td>
      <td>Frank Capra</td>
      <td>James Stewart</td>
      <td>Donna Reed</td>
      <td>Lionel Barrymore</td>
      <td>Thomas Mitchell</td>
      <td>405801</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>33</th>
      <td>Joker</td>
      <td>2019</td>
      <td>A</td>
      <td>122</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.5</td>
      <td>In Gotham City, mentally troubled comedian Art...</td>
      <td>59.00000</td>
      <td>Todd Phillips</td>
      <td>Joaquin Phoenix</td>
      <td>Robert De Niro</td>
      <td>Zazie Beetz</td>
      <td>Frances Conroy</td>
      <td>939252</td>
      <td>335451311</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Whiplash</td>
      <td>2014</td>
      <td>A</td>
      <td>106</td>
      <td>Drama, Music</td>
      <td>8.5</td>
      <td>A promising young drummer enrolls at a cut-thr...</td>
      <td>88.00000</td>
      <td>Damien Chazelle</td>
      <td>Miles Teller</td>
      <td>J.K. Simmons</td>
      <td>Melissa Benoist</td>
      <td>Paul Reiser</td>
      <td>717585</td>
      <td>13092000</td>
    </tr>
    <tr>
      <th>35</th>
      <td>The Intouchables</td>
      <td>2011</td>
      <td>UA</td>
      <td>112</td>
      <td>Biography, Comedy, Drama</td>
      <td>8.5</td>
      <td>After he becomes a quadriplegic from a paragli...</td>
      <td>57.00000</td>
      <td>Olivier Nakache</td>
      <td>Éric Toledano</td>
      <td>François Cluzet</td>
      <td>Omar Sy</td>
      <td>Anne Le Ny</td>
      <td>760360</td>
      <td>13182281</td>
    </tr>
    <tr>
      <th>36</th>
      <td>The Prestige</td>
      <td>2006</td>
      <td>U</td>
      <td>130</td>
      <td>Drama, Mystery, Sci-Fi</td>
      <td>8.5</td>
      <td>After a tragic accident, two stage magicians e...</td>
      <td>66.00000</td>
      <td>Christopher Nolan</td>
      <td>Christian Bale</td>
      <td>Hugh Jackman</td>
      <td>Scarlett Johansson</td>
      <td>Michael Caine</td>
      <td>1190259</td>
      <td>53089891</td>
    </tr>
    <tr>
      <th>37</th>
      <td>The Departed</td>
      <td>2006</td>
      <td>A</td>
      <td>151</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.5</td>
      <td>An undercover cop and a mole in the police att...</td>
      <td>85.00000</td>
      <td>Martin Scorsese</td>
      <td>Leonardo DiCaprio</td>
      <td>Matt Damon</td>
      <td>Jack Nicholson</td>
      <td>Mark Wahlberg</td>
      <td>1189773</td>
      <td>132384315</td>
    </tr>
    <tr>
      <th>38</th>
      <td>The Pianist</td>
      <td>2002</td>
      <td>R</td>
      <td>150</td>
      <td>Biography, Drama, Music</td>
      <td>8.5</td>
      <td>A Polish Jewish musician struggles to survive ...</td>
      <td>85.00000</td>
      <td>Roman Polanski</td>
      <td>Adrien Brody</td>
      <td>Thomas Kretschmann</td>
      <td>Frank Finlay</td>
      <td>Emilia Fox</td>
      <td>729603</td>
      <td>32572577</td>
    </tr>
    <tr>
      <th>39</th>
      <td>Gladiator</td>
      <td>2000</td>
      <td>UA</td>
      <td>155</td>
      <td>Action, Adventure, Drama</td>
      <td>8.5</td>
      <td>A former Roman General sets out to exact venge...</td>
      <td>67.00000</td>
      <td>Ridley Scott</td>
      <td>Russell Crowe</td>
      <td>Joaquin Phoenix</td>
      <td>Connie Nielsen</td>
      <td>Oliver Reed</td>
      <td>1341460</td>
      <td>187705427</td>
    </tr>
    <tr>
      <th>40</th>
      <td>American History X</td>
      <td>1998</td>
      <td>R</td>
      <td>119</td>
      <td>Drama</td>
      <td>8.5</td>
      <td>A former neo-nazi skinhead tries to prevent hi...</td>
      <td>62.00000</td>
      <td>Tony Kaye</td>
      <td>Edward Norton</td>
      <td>Edward Furlong</td>
      <td>Beverly D'Angelo</td>
      <td>Jennifer Lien</td>
      <td>1034705</td>
      <td>6719864</td>
    </tr>
    <tr>
      <th>41</th>
      <td>The Usual Suspects</td>
      <td>1995</td>
      <td>A</td>
      <td>106</td>
      <td>Crime, Mystery, Thriller</td>
      <td>8.5</td>
      <td>A sole survivor tells of the twisty events lea...</td>
      <td>77.00000</td>
      <td>Bryan Singer</td>
      <td>Kevin Spacey</td>
      <td>Gabriel Byrne</td>
      <td>Chazz Palminteri</td>
      <td>Stephen Baldwin</td>
      <td>991208</td>
      <td>23341568</td>
    </tr>
    <tr>
      <th>42</th>
      <td>Léon</td>
      <td>1994</td>
      <td>A</td>
      <td>110</td>
      <td>Action, Crime, Drama</td>
      <td>8.5</td>
      <td>Mathilda, a 12-year-old girl, is reluctantly t...</td>
      <td>64.00000</td>
      <td>Luc Besson</td>
      <td>Jean Reno</td>
      <td>Gary Oldman</td>
      <td>Natalie Portman</td>
      <td>Danny Aiello</td>
      <td>1035236</td>
      <td>19501238</td>
    </tr>
    <tr>
      <th>43</th>
      <td>The Lion King</td>
      <td>1994</td>
      <td>U</td>
      <td>88</td>
      <td>Animation, Adventure, Drama</td>
      <td>8.5</td>
      <td>Lion prince Simba and his father are targeted ...</td>
      <td>88.00000</td>
      <td>Roger Allers</td>
      <td>Rob Minkoff</td>
      <td>Matthew Broderick</td>
      <td>Jeremy Irons</td>
      <td>James Earl Jones</td>
      <td>942045</td>
      <td>422783777</td>
    </tr>
    <tr>
      <th>44</th>
      <td>Terminator 2: Judgment Day</td>
      <td>1991</td>
      <td>U</td>
      <td>137</td>
      <td>Action, Sci-Fi</td>
      <td>8.5</td>
      <td>A cyborg, identical to the one who failed to k...</td>
      <td>75.00000</td>
      <td>James Cameron</td>
      <td>Arnold Schwarzenegger</td>
      <td>Linda Hamilton</td>
      <td>Edward Furlong</td>
      <td>Robert Patrick</td>
      <td>995506</td>
      <td>204843350</td>
    </tr>
    <tr>
      <th>45</th>
      <td>Nuovo Cinema Paradiso</td>
      <td>1988</td>
      <td>U</td>
      <td>155</td>
      <td>Drama, Romance</td>
      <td>8.5</td>
      <td>A filmmaker recalls his childhood when falling...</td>
      <td>80.00000</td>
      <td>Giuseppe Tornatore</td>
      <td>Philippe Noiret</td>
      <td>Enzo Cannavale</td>
      <td>Antonella Attili</td>
      <td>Isa Danieli</td>
      <td>230763</td>
      <td>11990401</td>
    </tr>
    <tr>
      <th>46</th>
      <td>Hotaru no haka</td>
      <td>1988</td>
      <td>U</td>
      <td>89</td>
      <td>Animation, Drama, War</td>
      <td>8.5</td>
      <td>A young boy and his little sister struggle to ...</td>
      <td>94.00000</td>
      <td>Isao Takahata</td>
      <td>Tsutomu Tatsumi</td>
      <td>Ayano Shiraishi</td>
      <td>Akemi Yamaguchi</td>
      <td>Yoshiko Shinohara</td>
      <td>235231</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>47</th>
      <td>Back to the Future</td>
      <td>1985</td>
      <td>U</td>
      <td>116</td>
      <td>Adventure, Comedy, Sci-Fi</td>
      <td>8.5</td>
      <td>Marty McFly, a 17-year-old high school student...</td>
      <td>87.00000</td>
      <td>Robert Zemeckis</td>
      <td>Michael J. Fox</td>
      <td>Christopher Lloyd</td>
      <td>Lea Thompson</td>
      <td>Crispin Glover</td>
      <td>1058081</td>
      <td>210609762</td>
    </tr>
    <tr>
      <th>48</th>
      <td>Once Upon a Time in the West</td>
      <td>1968</td>
      <td>U</td>
      <td>165</td>
      <td>Western</td>
      <td>8.5</td>
      <td>A mysterious stranger with a harmonica joins f...</td>
      <td>80.00000</td>
      <td>Sergio Leone</td>
      <td>Henry Fonda</td>
      <td>Charles Bronson</td>
      <td>Claudia Cardinale</td>
      <td>Jason Robards</td>
      <td>302844</td>
      <td>5321508</td>
    </tr>
    <tr>
      <th>49</th>
      <td>Psycho</td>
      <td>1960</td>
      <td>A</td>
      <td>109</td>
      <td>Horror, Mystery, Thriller</td>
      <td>8.5</td>
      <td>A Phoenix secretary embezzles $40,000 from her...</td>
      <td>97.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Anthony Perkins</td>
      <td>Janet Leigh</td>
      <td>Vera Miles</td>
      <td>John Gavin</td>
      <td>604211</td>
      <td>32000000</td>
    </tr>
    <tr>
      <th>50</th>
      <td>Casablanca</td>
      <td>1942</td>
      <td>U</td>
      <td>102</td>
      <td>Drama, Romance, War</td>
      <td>8.5</td>
      <td>A cynical expatriate American cafe owner strug...</td>
      <td>100.00000</td>
      <td>Michael Curtiz</td>
      <td>Humphrey Bogart</td>
      <td>Ingrid Bergman</td>
      <td>Paul Henreid</td>
      <td>Claude Rains</td>
      <td>522093</td>
      <td>1024560</td>
    </tr>
    <tr>
      <th>51</th>
      <td>Modern Times</td>
      <td>1936</td>
      <td>G</td>
      <td>87</td>
      <td>Comedy, Drama, Family</td>
      <td>8.5</td>
      <td>The Tramp struggles to live in modern industri...</td>
      <td>96.00000</td>
      <td>Charles Chaplin</td>
      <td>Charles Chaplin</td>
      <td>Paulette Goddard</td>
      <td>Henry Bergman</td>
      <td>Tiny Sandford</td>
      <td>217881</td>
      <td>163245</td>
    </tr>
    <tr>
      <th>52</th>
      <td>City Lights</td>
      <td>1931</td>
      <td>G</td>
      <td>87</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.5</td>
      <td>With the aid of a wealthy erratic tippler, a d...</td>
      <td>99.00000</td>
      <td>Charles Chaplin</td>
      <td>Charles Chaplin</td>
      <td>Virginia Cherrill</td>
      <td>Florence Lee</td>
      <td>Harry Myers</td>
      <td>167839</td>
      <td>19181</td>
    </tr>
    <tr>
      <th>53</th>
      <td>Capharnaüm</td>
      <td>2018</td>
      <td>A</td>
      <td>126</td>
      <td>Drama</td>
      <td>8.4</td>
      <td>While serving a five-year sentence for a viole...</td>
      <td>75.00000</td>
      <td>Nadine Labaki</td>
      <td>Zain Al Rafeea</td>
      <td>Yordanos Shiferaw</td>
      <td>Boluwatife Treasure Bankole</td>
      <td>Kawsar Al Haddad</td>
      <td>62635</td>
      <td>1661096</td>
    </tr>
    <tr>
      <th>54</th>
      <td>Ayla: The Daughter of War</td>
      <td>2017</td>
      <td>Unknown</td>
      <td>125</td>
      <td>Biography, Drama, History</td>
      <td>8.4</td>
      <td>In 1950, amid-st the ravages of the Korean War...</td>
      <td>77.97153</td>
      <td>Can Ulkay</td>
      <td>Erdem Can</td>
      <td>Çetin Tekindor</td>
      <td>Ismail Hacioglu</td>
      <td>Kyung-jin Lee</td>
      <td>34112</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>55</th>
      <td>Vikram Vedha</td>
      <td>2017</td>
      <td>UA</td>
      <td>147</td>
      <td>Action, Crime, Drama</td>
      <td>8.4</td>
      <td>Vikram, a no-nonsense police officer, accompan...</td>
      <td>77.97153</td>
      <td>Gayatri</td>
      <td>Pushkar</td>
      <td>Madhavan</td>
      <td>Vijay Sethupathi</td>
      <td>Shraddha Srinath</td>
      <td>28401</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>56</th>
      <td>Kimi no na wa.</td>
      <td>2016</td>
      <td>U</td>
      <td>106</td>
      <td>Animation, Drama, Fantasy</td>
      <td>8.4</td>
      <td>Two strangers find themselves linked in a biza...</td>
      <td>79.00000</td>
      <td>Makoto Shinkai</td>
      <td>Ryûnosuke Kamiki</td>
      <td>Mone Kamishiraishi</td>
      <td>Ryô Narita</td>
      <td>Aoi Yûki</td>
      <td>194838</td>
      <td>5017246</td>
    </tr>
    <tr>
      <th>57</th>
      <td>Dangal</td>
      <td>2016</td>
      <td>U</td>
      <td>161</td>
      <td>Action, Biography, Drama</td>
      <td>8.4</td>
      <td>Former wrestler Mahavir Singh Phogat and his t...</td>
      <td>77.97153</td>
      <td>Nitesh Tiwari</td>
      <td>Aamir Khan</td>
      <td>Sakshi Tanwar</td>
      <td>Fatima Sana Shaikh</td>
      <td>Sanya Malhotra</td>
      <td>156479</td>
      <td>12391761</td>
    </tr>
    <tr>
      <th>58</th>
      <td>Spider-Man: Into the Spider-Verse</td>
      <td>2018</td>
      <td>U</td>
      <td>117</td>
      <td>Animation, Action, Adventure</td>
      <td>8.4</td>
      <td>Teen Miles Morales becomes the Spider-Man of h...</td>
      <td>87.00000</td>
      <td>Bob Persichetti</td>
      <td>Peter Ramsey</td>
      <td>Rodney Rothman</td>
      <td>Shameik Moore</td>
      <td>Jake Johnson</td>
      <td>375110</td>
      <td>190241310</td>
    </tr>
    <tr>
      <th>59</th>
      <td>Avengers: Endgame</td>
      <td>2019</td>
      <td>UA</td>
      <td>181</td>
      <td>Action, Adventure, Drama</td>
      <td>8.4</td>
      <td>After the devastating events of Avengers: Infi...</td>
      <td>78.00000</td>
      <td>Anthony Russo</td>
      <td>Joe Russo</td>
      <td>Robert Downey Jr.</td>
      <td>Chris Evans</td>
      <td>Mark Ruffalo</td>
      <td>809955</td>
      <td>858373000</td>
    </tr>
    <tr>
      <th>60</th>
      <td>Avengers: Infinity War</td>
      <td>2018</td>
      <td>UA</td>
      <td>149</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>8.4</td>
      <td>The Avengers and their allies must be willing ...</td>
      <td>68.00000</td>
      <td>Anthony Russo</td>
      <td>Joe Russo</td>
      <td>Robert Downey Jr.</td>
      <td>Chris Hemsworth</td>
      <td>Mark Ruffalo</td>
      <td>834477</td>
      <td>678815482</td>
    </tr>
    <tr>
      <th>61</th>
      <td>Coco</td>
      <td>2017</td>
      <td>U</td>
      <td>105</td>
      <td>Animation, Adventure, Family</td>
      <td>8.4</td>
      <td>Aspiring musician Miguel, confronted with his ...</td>
      <td>81.00000</td>
      <td>Lee Unkrich</td>
      <td>Adrian Molina</td>
      <td>Anthony Gonzalez</td>
      <td>Gael García Bernal</td>
      <td>Benjamin Bratt</td>
      <td>384171</td>
      <td>209726015</td>
    </tr>
    <tr>
      <th>62</th>
      <td>Django Unchained</td>
      <td>2012</td>
      <td>A</td>
      <td>165</td>
      <td>Drama, Western</td>
      <td>8.4</td>
      <td>With the help of a German bounty hunter, a fre...</td>
      <td>81.00000</td>
      <td>Quentin Tarantino</td>
      <td>Jamie Foxx</td>
      <td>Christoph Waltz</td>
      <td>Leonardo DiCaprio</td>
      <td>Kerry Washington</td>
      <td>1357682</td>
      <td>162805434</td>
    </tr>
    <tr>
      <th>63</th>
      <td>The Dark Knight Rises</td>
      <td>2012</td>
      <td>UA</td>
      <td>164</td>
      <td>Action, Adventure</td>
      <td>8.4</td>
      <td>Eight years after the Joker's reign of anarchy...</td>
      <td>78.00000</td>
      <td>Christopher Nolan</td>
      <td>Christian Bale</td>
      <td>Tom Hardy</td>
      <td>Anne Hathaway</td>
      <td>Gary Oldman</td>
      <td>1516346</td>
      <td>448139099</td>
    </tr>
    <tr>
      <th>64</th>
      <td>3 Idiots</td>
      <td>2009</td>
      <td>UA</td>
      <td>170</td>
      <td>Comedy, Drama</td>
      <td>8.4</td>
      <td>Two friends are searching for their long lost ...</td>
      <td>67.00000</td>
      <td>Rajkumar Hirani</td>
      <td>Aamir Khan</td>
      <td>Madhavan</td>
      <td>Mona Singh</td>
      <td>Sharman Joshi</td>
      <td>344445</td>
      <td>6532908</td>
    </tr>
    <tr>
      <th>65</th>
      <td>Taare Zameen Par</td>
      <td>2007</td>
      <td>U</td>
      <td>165</td>
      <td>Drama, Family</td>
      <td>8.4</td>
      <td>An eight-year-old boy is thought to be a lazy ...</td>
      <td>77.97153</td>
      <td>Aamir Khan</td>
      <td>Amole Gupte</td>
      <td>Darsheel Safary</td>
      <td>Aamir Khan</td>
      <td>Tisca Chopra</td>
      <td>168895</td>
      <td>1223869</td>
    </tr>
    <tr>
      <th>66</th>
      <td>WALL·E</td>
      <td>2008</td>
      <td>U</td>
      <td>98</td>
      <td>Animation, Adventure, Family</td>
      <td>8.4</td>
      <td>In the distant future, a small waste-collectin...</td>
      <td>95.00000</td>
      <td>Andrew Stanton</td>
      <td>Ben Burtt</td>
      <td>Elissa Knight</td>
      <td>Jeff Garlin</td>
      <td>Fred Willard</td>
      <td>999790</td>
      <td>223808164</td>
    </tr>
    <tr>
      <th>67</th>
      <td>The Lives of Others</td>
      <td>2006</td>
      <td>A</td>
      <td>137</td>
      <td>Drama, Mystery, Thriller</td>
      <td>8.4</td>
      <td>In 1984 East Berlin, an agent of the secret po...</td>
      <td>89.00000</td>
      <td>Florian Henckel von Donnersmarck</td>
      <td>Ulrich Mühe</td>
      <td>Martina Gedeck</td>
      <td>Sebastian Koch</td>
      <td>Ulrich Tukur</td>
      <td>358685</td>
      <td>11286112</td>
    </tr>
    <tr>
      <th>68</th>
      <td>Oldeuboi</td>
      <td>2003</td>
      <td>A</td>
      <td>101</td>
      <td>Action, Drama, Mystery</td>
      <td>8.4</td>
      <td>After being kidnapped and imprisoned for fifte...</td>
      <td>77.00000</td>
      <td>Chan-wook Park</td>
      <td>Choi Min-sik</td>
      <td>Yoo Ji-Tae</td>
      <td>Kang Hye-jeong</td>
      <td>Kim Byeong-Ok</td>
      <td>515451</td>
      <td>707481</td>
    </tr>
    <tr>
      <th>69</th>
      <td>Memento</td>
      <td>2000</td>
      <td>UA</td>
      <td>113</td>
      <td>Mystery, Thriller</td>
      <td>8.4</td>
      <td>A man with short-term memory loss attempts to ...</td>
      <td>80.00000</td>
      <td>Christopher Nolan</td>
      <td>Guy Pearce</td>
      <td>Carrie-Anne Moss</td>
      <td>Joe Pantoliano</td>
      <td>Mark Boone Junior</td>
      <td>1125712</td>
      <td>25544867</td>
    </tr>
    <tr>
      <th>70</th>
      <td>Mononoke-hime</td>
      <td>1997</td>
      <td>U</td>
      <td>134</td>
      <td>Animation, Action, Adventure</td>
      <td>8.4</td>
      <td>On a journey to find the cure for a Tatarigami...</td>
      <td>76.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Yôji Matsuda</td>
      <td>Yuriko Ishida</td>
      <td>Yûko Tanaka</td>
      <td>Billy Crudup</td>
      <td>343171</td>
      <td>2375308</td>
    </tr>
    <tr>
      <th>71</th>
      <td>Once Upon a Time in America</td>
      <td>1984</td>
      <td>A</td>
      <td>229</td>
      <td>Crime, Drama</td>
      <td>8.4</td>
      <td>A former Prohibition-era Jewish gangster retur...</td>
      <td>77.97153</td>
      <td>Sergio Leone</td>
      <td>Robert De Niro</td>
      <td>James Woods</td>
      <td>Elizabeth McGovern</td>
      <td>Treat Williams</td>
      <td>311365</td>
      <td>5321508</td>
    </tr>
    <tr>
      <th>72</th>
      <td>Raiders of the Lost Ark</td>
      <td>1981</td>
      <td>A</td>
      <td>115</td>
      <td>Action, Adventure</td>
      <td>8.4</td>
      <td>In 1936, archaeologist and adventurer Indiana ...</td>
      <td>85.00000</td>
      <td>Steven Spielberg</td>
      <td>Harrison Ford</td>
      <td>Karen Allen</td>
      <td>Paul Freeman</td>
      <td>John Rhys-Davies</td>
      <td>884112</td>
      <td>248159971</td>
    </tr>
    <tr>
      <th>73</th>
      <td>The Shining</td>
      <td>1980</td>
      <td>A</td>
      <td>146</td>
      <td>Drama, Horror</td>
      <td>8.4</td>
      <td>A family heads to an isolated hotel for the wi...</td>
      <td>66.00000</td>
      <td>Stanley Kubrick</td>
      <td>Jack Nicholson</td>
      <td>Shelley Duvall</td>
      <td>Danny Lloyd</td>
      <td>Scatman Crothers</td>
      <td>898237</td>
      <td>44017374</td>
    </tr>
    <tr>
      <th>74</th>
      <td>Apocalypse Now</td>
      <td>1979</td>
      <td>R</td>
      <td>147</td>
      <td>Drama, Mystery, War</td>
      <td>8.4</td>
      <td>A U.S. Army officer serving in Vietnam is task...</td>
      <td>94.00000</td>
      <td>Francis Ford Coppola</td>
      <td>Martin Sheen</td>
      <td>Marlon Brando</td>
      <td>Robert Duvall</td>
      <td>Frederic Forrest</td>
      <td>606398</td>
      <td>83471511</td>
    </tr>
    <tr>
      <th>75</th>
      <td>Alien</td>
      <td>1979</td>
      <td>R</td>
      <td>117</td>
      <td>Horror, Sci-Fi</td>
      <td>8.4</td>
      <td>After a space merchant vessel receives an unkn...</td>
      <td>89.00000</td>
      <td>Ridley Scott</td>
      <td>Sigourney Weaver</td>
      <td>Tom Skerritt</td>
      <td>John Hurt</td>
      <td>Veronica Cartwright</td>
      <td>787806</td>
      <td>78900000</td>
    </tr>
    <tr>
      <th>76</th>
      <td>Anand</td>
      <td>1971</td>
      <td>U</td>
      <td>122</td>
      <td>Drama, Musical</td>
      <td>8.4</td>
      <td>The story of a terminally ill man who wishes t...</td>
      <td>77.97153</td>
      <td>Hrishikesh Mukherjee</td>
      <td>Rajesh Khanna</td>
      <td>Amitabh Bachchan</td>
      <td>Sumita Sanyal</td>
      <td>Ramesh Deo</td>
      <td>30273</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>77</th>
      <td>Tengoku to jigoku</td>
      <td>1963</td>
      <td>Unknown</td>
      <td>143</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.4</td>
      <td>An executive of a shoe company becomes a victi...</td>
      <td>77.97153</td>
      <td>Akira Kurosawa</td>
      <td>Toshirô Mifune</td>
      <td>Yutaka Sada</td>
      <td>Tatsuya Nakadai</td>
      <td>Kyôko Kagawa</td>
      <td>34357</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>78</th>
      <td>Dr. Strangelove or: How I Learned to Stop Worr...</td>
      <td>1964</td>
      <td>A</td>
      <td>95</td>
      <td>Comedy</td>
      <td>8.4</td>
      <td>An insane general triggers a path to nuclear h...</td>
      <td>97.00000</td>
      <td>Stanley Kubrick</td>
      <td>Peter Sellers</td>
      <td>George C. Scott</td>
      <td>Sterling Hayden</td>
      <td>Keenan Wynn</td>
      <td>450474</td>
      <td>275902</td>
    </tr>
    <tr>
      <th>79</th>
      <td>Witness for the Prosecution</td>
      <td>1957</td>
      <td>U</td>
      <td>116</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.4</td>
      <td>A veteran British barrister must defend his cl...</td>
      <td>77.97153</td>
      <td>Billy Wilder</td>
      <td>Tyrone Power</td>
      <td>Marlene Dietrich</td>
      <td>Charles Laughton</td>
      <td>Elsa Lanchester</td>
      <td>108862</td>
      <td>8175000</td>
    </tr>
    <tr>
      <th>80</th>
      <td>Paths of Glory</td>
      <td>1957</td>
      <td>A</td>
      <td>88</td>
      <td>Drama, War</td>
      <td>8.4</td>
      <td>After refusing to attack an enemy position, a ...</td>
      <td>90.00000</td>
      <td>Stanley Kubrick</td>
      <td>Kirk Douglas</td>
      <td>Ralph Meeker</td>
      <td>Adolphe Menjou</td>
      <td>George Macready</td>
      <td>178092</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>81</th>
      <td>Rear Window</td>
      <td>1954</td>
      <td>U</td>
      <td>112</td>
      <td>Mystery, Thriller</td>
      <td>8.4</td>
      <td>A wheelchair-bound photographer spies on his n...</td>
      <td>100.00000</td>
      <td>Alfred Hitchcock</td>
      <td>James Stewart</td>
      <td>Grace Kelly</td>
      <td>Wendell Corey</td>
      <td>Thelma Ritter</td>
      <td>444074</td>
      <td>36764313</td>
    </tr>
    <tr>
      <th>82</th>
      <td>Sunset Blvd.</td>
      <td>1950</td>
      <td>Passed</td>
      <td>110</td>
      <td>Drama, Film-Noir</td>
      <td>8.4</td>
      <td>A screenwriter develops a dangerous relationsh...</td>
      <td>77.97153</td>
      <td>Billy Wilder</td>
      <td>William Holden</td>
      <td>Gloria Swanson</td>
      <td>Erich von Stroheim</td>
      <td>Nancy Olson</td>
      <td>201632</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>83</th>
      <td>The Great Dictator</td>
      <td>1940</td>
      <td>Passed</td>
      <td>125</td>
      <td>Comedy, Drama, War</td>
      <td>8.4</td>
      <td>Dictator Adenoid Hynkel tries to expand his em...</td>
      <td>77.97153</td>
      <td>Charles Chaplin</td>
      <td>Charles Chaplin</td>
      <td>Paulette Goddard</td>
      <td>Jack Oakie</td>
      <td>Reginald Gardiner</td>
      <td>203150</td>
      <td>288475</td>
    </tr>
    <tr>
      <th>84</th>
      <td>1917</td>
      <td>2019</td>
      <td>R</td>
      <td>119</td>
      <td>Drama, Thriller, War</td>
      <td>8.3</td>
      <td>April 6th, 1917. As a regiment assembles to wa...</td>
      <td>78.00000</td>
      <td>Sam Mendes</td>
      <td>Dean-Charles Chapman</td>
      <td>George MacKay</td>
      <td>Daniel Mays</td>
      <td>Colin Firth</td>
      <td>425844</td>
      <td>159227644</td>
    </tr>
    <tr>
      <th>85</th>
      <td>Tumbbad</td>
      <td>2018</td>
      <td>A</td>
      <td>104</td>
      <td>Drama, Fantasy, Horror</td>
      <td>8.3</td>
      <td>A mythological story about a goddess who creat...</td>
      <td>77.97153</td>
      <td>Rahi Anil Barve</td>
      <td>Anand Gandhi</td>
      <td>Adesh Prasad</td>
      <td>Sohum Shah</td>
      <td>Jyoti Malshe</td>
      <td>27793</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>86</th>
      <td>Andhadhun</td>
      <td>2018</td>
      <td>UA</td>
      <td>139</td>
      <td>Crime, Drama, Music</td>
      <td>8.3</td>
      <td>A series of mysterious events change the life ...</td>
      <td>77.97153</td>
      <td>Sriram Raghavan</td>
      <td>Ayushmann Khurrana</td>
      <td>Tabu</td>
      <td>Radhika Apte</td>
      <td>Anil Dhawan</td>
      <td>71875</td>
      <td>1373943</td>
    </tr>
    <tr>
      <th>87</th>
      <td>Drishyam</td>
      <td>2013</td>
      <td>U</td>
      <td>160</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.3</td>
      <td>A man goes to extreme lengths to save his fami...</td>
      <td>77.97153</td>
      <td>Jeethu Joseph</td>
      <td>Mohanlal</td>
      <td>Meena</td>
      <td>Asha Sharath</td>
      <td>Ansiba</td>
      <td>30722</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>88</th>
      <td>Jagten</td>
      <td>2012</td>
      <td>R</td>
      <td>115</td>
      <td>Drama</td>
      <td>8.3</td>
      <td>A teacher lives a lonely life, all the while s...</td>
      <td>77.00000</td>
      <td>Thomas Vinterberg</td>
      <td>Mads Mikkelsen</td>
      <td>Thomas Bo Larsen</td>
      <td>Annika Wedderkopp</td>
      <td>Lasse Fogelstrøm</td>
      <td>281623</td>
      <td>687185</td>
    </tr>
    <tr>
      <th>89</th>
      <td>Jodaeiye Nader az Simin</td>
      <td>2011</td>
      <td>PG-13</td>
      <td>123</td>
      <td>Drama</td>
      <td>8.3</td>
      <td>A married couple are faced with a difficult de...</td>
      <td>95.00000</td>
      <td>Asghar Farhadi</td>
      <td>Payman Maadi</td>
      <td>Leila Hatami</td>
      <td>Sareh Bayat</td>
      <td>Shahab Hosseini</td>
      <td>220002</td>
      <td>7098492</td>
    </tr>
    <tr>
      <th>90</th>
      <td>Incendies</td>
      <td>2010</td>
      <td>R</td>
      <td>131</td>
      <td>Drama, Mystery, War</td>
      <td>8.3</td>
      <td>Twins journey to the Middle East to discover t...</td>
      <td>80.00000</td>
      <td>Denis Villeneuve</td>
      <td>Lubna Azabal</td>
      <td>Mélissa Désormeaux-Poulin</td>
      <td>Maxim Gaudette</td>
      <td>Mustafa Kamel</td>
      <td>150023</td>
      <td>6857096</td>
    </tr>
    <tr>
      <th>91</th>
      <td>Miracle in cell NO.7</td>
      <td>2019</td>
      <td>TV-14</td>
      <td>132</td>
      <td>Drama</td>
      <td>8.3</td>
      <td>A story of love between a mentally-ill father ...</td>
      <td>77.97153</td>
      <td>Mehmet Ada Öztekin</td>
      <td>Aras Bulut Iynemli</td>
      <td>Nisa Sofiya Aksongur</td>
      <td>Deniz Baysal</td>
      <td>Celile Toyon Uysal</td>
      <td>33935</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>92</th>
      <td>Babam ve Oglum</td>
      <td>2005</td>
      <td>Unknown</td>
      <td>112</td>
      <td>Drama, Family</td>
      <td>8.3</td>
      <td>The family of a left-wing journalist is torn a...</td>
      <td>77.97153</td>
      <td>Çagan Irmak</td>
      <td>Çetin Tekindor</td>
      <td>Fikret Kuskan</td>
      <td>Hümeyra</td>
      <td>Ege Tanman</td>
      <td>78925</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>93</th>
      <td>Inglourious Basterds</td>
      <td>2009</td>
      <td>A</td>
      <td>153</td>
      <td>Adventure, Drama, War</td>
      <td>8.3</td>
      <td>In Nazi-occupied France during World War II, a...</td>
      <td>69.00000</td>
      <td>Quentin Tarantino</td>
      <td>Brad Pitt</td>
      <td>Diane Kruger</td>
      <td>Eli Roth</td>
      <td>Mélanie Laurent</td>
      <td>1267869</td>
      <td>120540719</td>
    </tr>
    <tr>
      <th>94</th>
      <td>Eternal Sunshine of the Spotless Mind</td>
      <td>2004</td>
      <td>UA</td>
      <td>108</td>
      <td>Drama, Romance, Sci-Fi</td>
      <td>8.3</td>
      <td>When their relationship turns sour, a couple u...</td>
      <td>89.00000</td>
      <td>Michel Gondry</td>
      <td>Jim Carrey</td>
      <td>Kate Winslet</td>
      <td>Tom Wilkinson</td>
      <td>Gerry Robert Byrne</td>
      <td>911664</td>
      <td>34400301</td>
    </tr>
    <tr>
      <th>95</th>
      <td>Amélie</td>
      <td>2001</td>
      <td>U</td>
      <td>122</td>
      <td>Comedy, Romance</td>
      <td>8.3</td>
      <td>Amélie is an innocent and naive girl in Paris ...</td>
      <td>69.00000</td>
      <td>Jean-Pierre Jeunet</td>
      <td>Audrey Tautou</td>
      <td>Mathieu Kassovitz</td>
      <td>Rufus</td>
      <td>Lorella Cravotta</td>
      <td>703810</td>
      <td>33225499</td>
    </tr>
    <tr>
      <th>96</th>
      <td>Snatch</td>
      <td>2000</td>
      <td>UA</td>
      <td>104</td>
      <td>Comedy, Crime</td>
      <td>8.3</td>
      <td>Unscrupulous boxing promoters, violent bookmak...</td>
      <td>55.00000</td>
      <td>Guy Ritchie</td>
      <td>Jason Statham</td>
      <td>Brad Pitt</td>
      <td>Benicio Del Toro</td>
      <td>Dennis Farina</td>
      <td>782001</td>
      <td>30328156</td>
    </tr>
    <tr>
      <th>97</th>
      <td>Requiem for a Dream</td>
      <td>2000</td>
      <td>A</td>
      <td>102</td>
      <td>Drama</td>
      <td>8.3</td>
      <td>The drug-induced utopias of four Coney Island ...</td>
      <td>68.00000</td>
      <td>Darren Aronofsky</td>
      <td>Ellen Burstyn</td>
      <td>Jared Leto</td>
      <td>Jennifer Connelly</td>
      <td>Marlon Wayans</td>
      <td>766870</td>
      <td>3635482</td>
    </tr>
    <tr>
      <th>98</th>
      <td>American Beauty</td>
      <td>1999</td>
      <td>UA</td>
      <td>122</td>
      <td>Drama</td>
      <td>8.3</td>
      <td>A sexually frustrated suburban father has a mi...</td>
      <td>84.00000</td>
      <td>Sam Mendes</td>
      <td>Kevin Spacey</td>
      <td>Annette Bening</td>
      <td>Thora Birch</td>
      <td>Wes Bentley</td>
      <td>1069738</td>
      <td>130096601</td>
    </tr>
    <tr>
      <th>99</th>
      <td>Good Will Hunting</td>
      <td>1997</td>
      <td>U</td>
      <td>126</td>
      <td>Drama, Romance</td>
      <td>8.3</td>
      <td>Will Hunting, a janitor at M.I.T., has a gift ...</td>
      <td>70.00000</td>
      <td>Gus Van Sant</td>
      <td>Robin Williams</td>
      <td>Matt Damon</td>
      <td>Ben Affleck</td>
      <td>Stellan Skarsgård</td>
      <td>861606</td>
      <td>138433435</td>
    </tr>
    <tr>
      <th>100</th>
      <td>Bacheha-Ye aseman</td>
      <td>1997</td>
      <td>PG</td>
      <td>89</td>
      <td>Drama, Family, Sport</td>
      <td>8.3</td>
      <td>After a boy loses his sister's pair of shoes, ...</td>
      <td>77.00000</td>
      <td>Majid Majidi</td>
      <td>Mohammad Amir Naji</td>
      <td>Amir Farrokh Hashemian</td>
      <td>Bahare Seddiqi</td>
      <td>Nafise Jafar-Mohammadi</td>
      <td>65341</td>
      <td>933933</td>
    </tr>
    <tr>
      <th>101</th>
      <td>Toy Story</td>
      <td>1995</td>
      <td>U</td>
      <td>81</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.3</td>
      <td>A cowboy doll is profoundly threatened and jea...</td>
      <td>95.00000</td>
      <td>John Lasseter</td>
      <td>Tom Hanks</td>
      <td>Tim Allen</td>
      <td>Don Rickles</td>
      <td>Jim Varney</td>
      <td>887429</td>
      <td>191796233</td>
    </tr>
    <tr>
      <th>102</th>
      <td>Braveheart</td>
      <td>1995</td>
      <td>A</td>
      <td>178</td>
      <td>Biography, Drama, History</td>
      <td>8.3</td>
      <td>Scottish warrior William Wallace leads his cou...</td>
      <td>68.00000</td>
      <td>Mel Gibson</td>
      <td>Mel Gibson</td>
      <td>Sophie Marceau</td>
      <td>Patrick McGoohan</td>
      <td>Angus Macfadyen</td>
      <td>959181</td>
      <td>75600000</td>
    </tr>
    <tr>
      <th>103</th>
      <td>Reservoir Dogs</td>
      <td>1992</td>
      <td>R</td>
      <td>99</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.3</td>
      <td>When a simple jewelry heist goes horribly wron...</td>
      <td>79.00000</td>
      <td>Quentin Tarantino</td>
      <td>Harvey Keitel</td>
      <td>Tim Roth</td>
      <td>Michael Madsen</td>
      <td>Chris Penn</td>
      <td>918562</td>
      <td>2832029</td>
    </tr>
    <tr>
      <th>104</th>
      <td>Full Metal Jacket</td>
      <td>1987</td>
      <td>UA</td>
      <td>116</td>
      <td>Drama, War</td>
      <td>8.3</td>
      <td>A pragmatic U.S. Marine observes the dehumaniz...</td>
      <td>76.00000</td>
      <td>Stanley Kubrick</td>
      <td>Matthew Modine</td>
      <td>R. Lee Ermey</td>
      <td>Vincent D'Onofrio</td>
      <td>Adam Baldwin</td>
      <td>675146</td>
      <td>46357676</td>
    </tr>
    <tr>
      <th>105</th>
      <td>Idi i smotri</td>
      <td>1985</td>
      <td>A</td>
      <td>142</td>
      <td>Drama, Thriller, War</td>
      <td>8.3</td>
      <td>After finding an old rifle, a young boy joins ...</td>
      <td>77.97153</td>
      <td>Elem Klimov</td>
      <td>Aleksey Kravchenko</td>
      <td>Olga Mironova</td>
      <td>Liubomiras Laucevicius</td>
      <td>Vladas Bagdonas</td>
      <td>59056</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>106</th>
      <td>Aliens</td>
      <td>1986</td>
      <td>U</td>
      <td>137</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>8.3</td>
      <td>Fifty-seven years after surviving an apocalypt...</td>
      <td>84.00000</td>
      <td>James Cameron</td>
      <td>Sigourney Weaver</td>
      <td>Michael Biehn</td>
      <td>Carrie Henn</td>
      <td>Paul Reiser</td>
      <td>652719</td>
      <td>85160248</td>
    </tr>
    <tr>
      <th>107</th>
      <td>Amadeus</td>
      <td>1984</td>
      <td>R</td>
      <td>160</td>
      <td>Biography, Drama, History</td>
      <td>8.3</td>
      <td>The life, success and troubles of Wolfgang Ama...</td>
      <td>88.00000</td>
      <td>Milos Forman</td>
      <td>F. Murray Abraham</td>
      <td>Tom Hulce</td>
      <td>Elizabeth Berridge</td>
      <td>Roy Dotrice</td>
      <td>369007</td>
      <td>51973029</td>
    </tr>
    <tr>
      <th>108</th>
      <td>Scarface</td>
      <td>1983</td>
      <td>A</td>
      <td>170</td>
      <td>Crime, Drama</td>
      <td>8.3</td>
      <td>In 1980 Miami, a determined Cuban immigrant ta...</td>
      <td>65.00000</td>
      <td>Brian De Palma</td>
      <td>Al Pacino</td>
      <td>Michelle Pfeiffer</td>
      <td>Steven Bauer</td>
      <td>Mary Elizabeth Mastrantonio</td>
      <td>740911</td>
      <td>45598982</td>
    </tr>
    <tr>
      <th>109</th>
      <td>Star Wars: Episode VI - Return of the Jedi</td>
      <td>1983</td>
      <td>U</td>
      <td>131</td>
      <td>Action, Adventure, Fantasy</td>
      <td>8.3</td>
      <td>After a daring mission to rescue Han Solo from...</td>
      <td>58.00000</td>
      <td>Richard Marquand</td>
      <td>Mark Hamill</td>
      <td>Harrison Ford</td>
      <td>Carrie Fisher</td>
      <td>Billy Dee Williams</td>
      <td>950470</td>
      <td>309125409</td>
    </tr>
    <tr>
      <th>110</th>
      <td>Das Boot</td>
      <td>1981</td>
      <td>R</td>
      <td>149</td>
      <td>Adventure, Drama, Thriller</td>
      <td>8.3</td>
      <td>The claustrophobic world of a WWII German U-bo...</td>
      <td>86.00000</td>
      <td>Wolfgang Petersen</td>
      <td>Jürgen Prochnow</td>
      <td>Herbert Grönemeyer</td>
      <td>Klaus Wennemann</td>
      <td>Hubertus Bengsch</td>
      <td>231855</td>
      <td>11487676</td>
    </tr>
    <tr>
      <th>111</th>
      <td>Taxi Driver</td>
      <td>1976</td>
      <td>A</td>
      <td>114</td>
      <td>Crime, Drama</td>
      <td>8.3</td>
      <td>A mentally unstable veteran works as a nightti...</td>
      <td>94.00000</td>
      <td>Martin Scorsese</td>
      <td>Robert De Niro</td>
      <td>Jodie Foster</td>
      <td>Cybill Shepherd</td>
      <td>Albert Brooks</td>
      <td>724636</td>
      <td>28262574</td>
    </tr>
    <tr>
      <th>112</th>
      <td>The Sting</td>
      <td>1973</td>
      <td>U</td>
      <td>129</td>
      <td>Comedy, Crime, Drama</td>
      <td>8.3</td>
      <td>Two grifters team up to pull off the ultimate ...</td>
      <td>83.00000</td>
      <td>George Roy Hill</td>
      <td>Paul Newman</td>
      <td>Robert Redford</td>
      <td>Robert Shaw</td>
      <td>Charles Durning</td>
      <td>241513</td>
      <td>159600000</td>
    </tr>
    <tr>
      <th>113</th>
      <td>A Clockwork Orange</td>
      <td>1971</td>
      <td>A</td>
      <td>136</td>
      <td>Crime, Drama, Sci-Fi</td>
      <td>8.3</td>
      <td>In the future, a sadistic gang leader is impri...</td>
      <td>77.00000</td>
      <td>Stanley Kubrick</td>
      <td>Malcolm McDowell</td>
      <td>Patrick Magee</td>
      <td>Michael Bates</td>
      <td>Warren Clarke</td>
      <td>757904</td>
      <td>6207725</td>
    </tr>
    <tr>
      <th>114</th>
      <td>2001: A Space Odyssey</td>
      <td>1968</td>
      <td>U</td>
      <td>149</td>
      <td>Adventure, Sci-Fi</td>
      <td>8.3</td>
      <td>After discovering a mysterious artifact buried...</td>
      <td>84.00000</td>
      <td>Stanley Kubrick</td>
      <td>Keir Dullea</td>
      <td>Gary Lockwood</td>
      <td>William Sylvester</td>
      <td>Daniel Richter</td>
      <td>603517</td>
      <td>56954992</td>
    </tr>
    <tr>
      <th>115</th>
      <td>Per qualche dollaro in più</td>
      <td>1965</td>
      <td>U</td>
      <td>132</td>
      <td>Western</td>
      <td>8.3</td>
      <td>Two bounty hunters with the same intentions te...</td>
      <td>74.00000</td>
      <td>Sergio Leone</td>
      <td>Clint Eastwood</td>
      <td>Lee Van Cleef</td>
      <td>Gian Maria Volontè</td>
      <td>Mara Krupp</td>
      <td>232772</td>
      <td>15000000</td>
    </tr>
    <tr>
      <th>116</th>
      <td>Lawrence of Arabia</td>
      <td>1962</td>
      <td>U</td>
      <td>228</td>
      <td>Adventure, Biography, Drama</td>
      <td>8.3</td>
      <td>The story of T.E. Lawrence, the English office...</td>
      <td>100.00000</td>
      <td>David Lean</td>
      <td>Peter O'Toole</td>
      <td>Alec Guinness</td>
      <td>Anthony Quinn</td>
      <td>Jack Hawkins</td>
      <td>268085</td>
      <td>44824144</td>
    </tr>
    <tr>
      <th>117</th>
      <td>The Apartment</td>
      <td>1960</td>
      <td>U</td>
      <td>125</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.3</td>
      <td>A man tries to rise in his company by letting ...</td>
      <td>94.00000</td>
      <td>Billy Wilder</td>
      <td>Jack Lemmon</td>
      <td>Shirley MacLaine</td>
      <td>Fred MacMurray</td>
      <td>Ray Walston</td>
      <td>164363</td>
      <td>18600000</td>
    </tr>
    <tr>
      <th>118</th>
      <td>North by Northwest</td>
      <td>1959</td>
      <td>U</td>
      <td>136</td>
      <td>Adventure, Mystery, Thriller</td>
      <td>8.3</td>
      <td>A New York City advertising executive goes on ...</td>
      <td>98.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Cary Grant</td>
      <td>Eva Marie Saint</td>
      <td>James Mason</td>
      <td>Jessie Royce Landis</td>
      <td>299198</td>
      <td>13275000</td>
    </tr>
    <tr>
      <th>119</th>
      <td>Vertigo</td>
      <td>1958</td>
      <td>A</td>
      <td>128</td>
      <td>Mystery, Romance, Thriller</td>
      <td>8.3</td>
      <td>A former police detective juggles wrestling wi...</td>
      <td>100.00000</td>
      <td>Alfred Hitchcock</td>
      <td>James Stewart</td>
      <td>Kim Novak</td>
      <td>Barbara Bel Geddes</td>
      <td>Tom Helmore</td>
      <td>364368</td>
      <td>3200000</td>
    </tr>
    <tr>
      <th>120</th>
      <td>Singin' in the Rain</td>
      <td>1952</td>
      <td>G</td>
      <td>103</td>
      <td>Comedy, Musical, Romance</td>
      <td>8.3</td>
      <td>A silent film production company and cast make...</td>
      <td>99.00000</td>
      <td>Stanley Donen</td>
      <td>Gene Kelly</td>
      <td>Gene Kelly</td>
      <td>Donald O'Connor</td>
      <td>Debbie Reynolds</td>
      <td>218957</td>
      <td>8819028</td>
    </tr>
    <tr>
      <th>121</th>
      <td>Ikiru</td>
      <td>1952</td>
      <td>Unknown</td>
      <td>143</td>
      <td>Drama</td>
      <td>8.3</td>
      <td>A bureaucrat tries to find a meaning in his li...</td>
      <td>77.97153</td>
      <td>Akira Kurosawa</td>
      <td>Takashi Shimura</td>
      <td>Nobuo Kaneko</td>
      <td>Shin'ichi Himori</td>
      <td>Haruo Tanaka</td>
      <td>68463</td>
      <td>55240</td>
    </tr>
    <tr>
      <th>122</th>
      <td>Ladri di biciclette</td>
      <td>1948</td>
      <td>Unknown</td>
      <td>89</td>
      <td>Drama</td>
      <td>8.3</td>
      <td>In post-war Italy, a working-class man's bicyc...</td>
      <td>77.97153</td>
      <td>Vittorio De Sica</td>
      <td>Lamberto Maggiorani</td>
      <td>Enzo Staiola</td>
      <td>Lianella Carell</td>
      <td>Elena Altieri</td>
      <td>146427</td>
      <td>332930</td>
    </tr>
    <tr>
      <th>123</th>
      <td>Double Indemnity</td>
      <td>1944</td>
      <td>Passed</td>
      <td>107</td>
      <td>Crime, Drama, Film-Noir</td>
      <td>8.3</td>
      <td>An insurance representative lets himself be ta...</td>
      <td>95.00000</td>
      <td>Billy Wilder</td>
      <td>Fred MacMurray</td>
      <td>Barbara Stanwyck</td>
      <td>Edward G. Robinson</td>
      <td>Byron Barr</td>
      <td>143525</td>
      <td>5720000</td>
    </tr>
    <tr>
      <th>124</th>
      <td>Citizen Kane</td>
      <td>1941</td>
      <td>UA</td>
      <td>119</td>
      <td>Drama, Mystery</td>
      <td>8.3</td>
      <td>Following the death of publishing tycoon Charl...</td>
      <td>100.00000</td>
      <td>Orson Welles</td>
      <td>Orson Welles</td>
      <td>Joseph Cotten</td>
      <td>Dorothy Comingore</td>
      <td>Agnes Moorehead</td>
      <td>403351</td>
      <td>1585634</td>
    </tr>
    <tr>
      <th>125</th>
      <td>M - Eine Stadt sucht einen Mörder</td>
      <td>1931</td>
      <td>Passed</td>
      <td>117</td>
      <td>Crime, Mystery, Thriller</td>
      <td>8.3</td>
      <td>When the police in a German city are unable to...</td>
      <td>77.97153</td>
      <td>Fritz Lang</td>
      <td>Peter Lorre</td>
      <td>Ellen Widmann</td>
      <td>Inge Landgut</td>
      <td>Otto Wernicke</td>
      <td>143434</td>
      <td>28877</td>
    </tr>
    <tr>
      <th>126</th>
      <td>Metropolis</td>
      <td>1927</td>
      <td>Unknown</td>
      <td>153</td>
      <td>Drama, Sci-Fi</td>
      <td>8.3</td>
      <td>In a futuristic city sharply divided between t...</td>
      <td>98.00000</td>
      <td>Fritz Lang</td>
      <td>Brigitte Helm</td>
      <td>Alfred Abel</td>
      <td>Gustav Fröhlich</td>
      <td>Rudolf Klein-Rogge</td>
      <td>159992</td>
      <td>1236166</td>
    </tr>
    <tr>
      <th>127</th>
      <td>The Kid</td>
      <td>1921</td>
      <td>Passed</td>
      <td>68</td>
      <td>Comedy, Drama, Family</td>
      <td>8.3</td>
      <td>The Tramp cares for an abandoned child, but ev...</td>
      <td>77.97153</td>
      <td>Charles Chaplin</td>
      <td>Charles Chaplin</td>
      <td>Edna Purviance</td>
      <td>Jackie Coogan</td>
      <td>Carl Miller</td>
      <td>113314</td>
      <td>5450000</td>
    </tr>
    <tr>
      <th>128</th>
      <td>Chhichhore</td>
      <td>2019</td>
      <td>UA</td>
      <td>143</td>
      <td>Comedy, Drama</td>
      <td>8.2</td>
      <td>A tragic incident forces Anirudh, a middle-age...</td>
      <td>77.97153</td>
      <td>Nitesh Tiwari</td>
      <td>Sushant Singh Rajput</td>
      <td>Shraddha Kapoor</td>
      <td>Varun Sharma</td>
      <td>Prateik</td>
      <td>33893</td>
      <td>898575</td>
    </tr>
    <tr>
      <th>129</th>
      <td>Uri: The Surgical Strike</td>
      <td>2018</td>
      <td>UA</td>
      <td>138</td>
      <td>Action, Drama, War</td>
      <td>8.2</td>
      <td>Indian army special forces execute a covert op...</td>
      <td>77.97153</td>
      <td>Aditya Dhar</td>
      <td>Vicky Kaushal</td>
      <td>Paresh Rawal</td>
      <td>Mohit Raina</td>
      <td>Yami Gautam</td>
      <td>43444</td>
      <td>4186168</td>
    </tr>
    <tr>
      <th>130</th>
      <td>K.G.F: Chapter 1</td>
      <td>2018</td>
      <td>UA</td>
      <td>156</td>
      <td>Action, Drama</td>
      <td>8.2</td>
      <td>In the 1970s, a fierce rebel rises against bru...</td>
      <td>77.97153</td>
      <td>Prashanth Neel</td>
      <td>Yash</td>
      <td>Srinidhi Shetty</td>
      <td>Ramachandra Raju</td>
      <td>Archana Jois</td>
      <td>36680</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>131</th>
      <td>Green Book</td>
      <td>2018</td>
      <td>UA</td>
      <td>130</td>
      <td>Biography, Comedy, Drama</td>
      <td>8.2</td>
      <td>A working-class Italian-American bouncer becom...</td>
      <td>69.00000</td>
      <td>Peter Farrelly</td>
      <td>Viggo Mortensen</td>
      <td>Mahershala Ali</td>
      <td>Linda Cardellini</td>
      <td>Sebastian Maniscalco</td>
      <td>377884</td>
      <td>85080171</td>
    </tr>
    <tr>
      <th>132</th>
      <td>Three Billboards Outside Ebbing, Missouri</td>
      <td>2017</td>
      <td>A</td>
      <td>115</td>
      <td>Comedy, Crime, Drama</td>
      <td>8.2</td>
      <td>A mother personally challenges the local autho...</td>
      <td>88.00000</td>
      <td>Martin McDonagh</td>
      <td>Frances McDormand</td>
      <td>Woody Harrelson</td>
      <td>Sam Rockwell</td>
      <td>Caleb Landry Jones</td>
      <td>432610</td>
      <td>54513740</td>
    </tr>
    <tr>
      <th>133</th>
      <td>Talvar</td>
      <td>2015</td>
      <td>UA</td>
      <td>132</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.2</td>
      <td>An experienced investigator confronts several ...</td>
      <td>77.97153</td>
      <td>Meghna Gulzar</td>
      <td>Irrfan Khan</td>
      <td>Konkona Sen Sharma</td>
      <td>Neeraj Kabi</td>
      <td>Sohum Shah</td>
      <td>31142</td>
      <td>342370</td>
    </tr>
    <tr>
      <th>134</th>
      <td>Baahubali 2: The Conclusion</td>
      <td>2017</td>
      <td>UA</td>
      <td>167</td>
      <td>Action, Drama</td>
      <td>8.2</td>
      <td>When Shiva, the son of Bahubali, learns about ...</td>
      <td>77.97153</td>
      <td>S.S. Rajamouli</td>
      <td>Prabhas</td>
      <td>Rana Daggubati</td>
      <td>Anushka Shetty</td>
      <td>Tamannaah Bhatia</td>
      <td>75348</td>
      <td>20186659</td>
    </tr>
    <tr>
      <th>135</th>
      <td>Klaus</td>
      <td>2019</td>
      <td>PG</td>
      <td>96</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.2</td>
      <td>A simple act of kindness always sparks another...</td>
      <td>65.00000</td>
      <td>Sergio Pablos</td>
      <td>Carlos Martínez López</td>
      <td>Jason Schwartzman</td>
      <td>J.K. Simmons</td>
      <td>Rashida Jones</td>
      <td>104761</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>136</th>
      <td>Drishyam</td>
      <td>2015</td>
      <td>UA</td>
      <td>163</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.2</td>
      <td>Desperate measures are taken by a man who trie...</td>
      <td>77.97153</td>
      <td>Nishikant Kamat</td>
      <td>Ajay Devgn</td>
      <td>Shriya Saran</td>
      <td>Tabu</td>
      <td>Rajat Kapoor</td>
      <td>70367</td>
      <td>739478</td>
    </tr>
    <tr>
      <th>137</th>
      <td>Queen</td>
      <td>2013</td>
      <td>UA</td>
      <td>146</td>
      <td>Adventure, Comedy, Drama</td>
      <td>8.2</td>
      <td>A Delhi girl from a traditional family sets ou...</td>
      <td>77.97153</td>
      <td>Vikas Bahl</td>
      <td>Kangana Ranaut</td>
      <td>Rajkummar Rao</td>
      <td>Lisa Haydon</td>
      <td>Jeffrey Ho</td>
      <td>60701</td>
      <td>1429534</td>
    </tr>
    <tr>
      <th>138</th>
      <td>Mandariinid</td>
      <td>2013</td>
      <td>Unknown</td>
      <td>87</td>
      <td>Drama, War</td>
      <td>8.2</td>
      <td>In 1992, war rages in Abkhazia, a breakaway re...</td>
      <td>73.00000</td>
      <td>Zaza Urushadze</td>
      <td>Lembit Ulfsak</td>
      <td>Elmo Nüganen</td>
      <td>Giorgi Nakashidze</td>
      <td>Misha Meskhi</td>
      <td>40382</td>
      <td>144501</td>
    </tr>
    <tr>
      <th>139</th>
      <td>Bhaag Milkha Bhaag</td>
      <td>2013</td>
      <td>U</td>
      <td>186</td>
      <td>Biography, Drama, Sport</td>
      <td>8.2</td>
      <td>The truth behind the ascension of Milkha Singh...</td>
      <td>77.97153</td>
      <td>Rakeysh Omprakash Mehra</td>
      <td>Farhan Akhtar</td>
      <td>Sonam Kapoor</td>
      <td>Pawan Malhotra</td>
      <td>Art Malik</td>
      <td>61137</td>
      <td>1626289</td>
    </tr>
    <tr>
      <th>140</th>
      <td>Gangs of Wasseypur</td>
      <td>2012</td>
      <td>A</td>
      <td>321</td>
      <td>Action, Comedy, Crime</td>
      <td>8.2</td>
      <td>A clash between Sultan and Shahid Khan leads t...</td>
      <td>89.00000</td>
      <td>Anurag Kashyap</td>
      <td>Manoj Bajpayee</td>
      <td>Richa Chadha</td>
      <td>Nawazuddin Siddiqui</td>
      <td>Tigmanshu Dhulia</td>
      <td>82365</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>141</th>
      <td>Udaan</td>
      <td>2010</td>
      <td>UA</td>
      <td>134</td>
      <td>Drama</td>
      <td>8.2</td>
      <td>Expelled from his school, a 16-year old boy re...</td>
      <td>77.97153</td>
      <td>Vikramaditya Motwane</td>
      <td>Rajat Barmecha</td>
      <td>Ronit Roy</td>
      <td>Manjot Singh</td>
      <td>Ram Kapoor</td>
      <td>42341</td>
      <td>7461</td>
    </tr>
    <tr>
      <th>142</th>
      <td>Paan Singh Tomar</td>
      <td>2012</td>
      <td>UA</td>
      <td>135</td>
      <td>Action, Biography, Crime</td>
      <td>8.2</td>
      <td>The story of Paan Singh Tomar, an Indian athle...</td>
      <td>77.97153</td>
      <td>Tigmanshu Dhulia</td>
      <td>Irrfan Khan</td>
      <td>Mahie Gill</td>
      <td>Rajesh Abhay</td>
      <td>Hemendra Dandotiya</td>
      <td>33237</td>
      <td>39567</td>
    </tr>
    <tr>
      <th>143</th>
      <td>El secreto de sus ojos</td>
      <td>2009</td>
      <td>R</td>
      <td>129</td>
      <td>Drama, Mystery, Romance</td>
      <td>8.2</td>
      <td>A retired legal counselor writes a novel hopin...</td>
      <td>80.00000</td>
      <td>Juan José Campanella</td>
      <td>Ricardo Darín</td>
      <td>Soledad Villamil</td>
      <td>Pablo Rago</td>
      <td>Carla Quevedo</td>
      <td>193217</td>
      <td>6391436</td>
    </tr>
    <tr>
      <th>144</th>
      <td>Warrior</td>
      <td>2011</td>
      <td>UA</td>
      <td>140</td>
      <td>Action, Drama, Sport</td>
      <td>8.2</td>
      <td>The youngest son of an alcoholic former boxer ...</td>
      <td>71.00000</td>
      <td>Gavin O'Connor</td>
      <td>Tom Hardy</td>
      <td>Nick Nolte</td>
      <td>Joel Edgerton</td>
      <td>Jennifer Morrison</td>
      <td>435950</td>
      <td>13657115</td>
    </tr>
    <tr>
      <th>145</th>
      <td>Shutter Island</td>
      <td>2010</td>
      <td>A</td>
      <td>138</td>
      <td>Mystery, Thriller</td>
      <td>8.2</td>
      <td>In 1954, a U.S. Marshal investigates the disap...</td>
      <td>63.00000</td>
      <td>Martin Scorsese</td>
      <td>Leonardo DiCaprio</td>
      <td>Emily Mortimer</td>
      <td>Mark Ruffalo</td>
      <td>Ben Kingsley</td>
      <td>1129894</td>
      <td>128012934</td>
    </tr>
    <tr>
      <th>146</th>
      <td>Up</td>
      <td>2009</td>
      <td>U</td>
      <td>96</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.2</td>
      <td>78-year-old Carl Fredricksen travels to Paradi...</td>
      <td>88.00000</td>
      <td>Pete Docter</td>
      <td>Bob Peterson</td>
      <td>Edward Asner</td>
      <td>Jordan Nagai</td>
      <td>John Ratzenberger</td>
      <td>935507</td>
      <td>293004164</td>
    </tr>
    <tr>
      <th>147</th>
      <td>The Wolf of Wall Street</td>
      <td>2013</td>
      <td>A</td>
      <td>180</td>
      <td>Biography, Crime, Drama</td>
      <td>8.2</td>
      <td>Based on the true story of Jordan Belfort, fro...</td>
      <td>75.00000</td>
      <td>Martin Scorsese</td>
      <td>Leonardo DiCaprio</td>
      <td>Jonah Hill</td>
      <td>Margot Robbie</td>
      <td>Matthew McConaughey</td>
      <td>1187498</td>
      <td>116900694</td>
    </tr>
    <tr>
      <th>148</th>
      <td>Chak De! India</td>
      <td>2007</td>
      <td>U</td>
      <td>153</td>
      <td>Drama, Family, Sport</td>
      <td>8.2</td>
      <td>Kabir Khan is the coach of the Indian Women's ...</td>
      <td>68.00000</td>
      <td>Shimit Amin</td>
      <td>Shah Rukh Khan</td>
      <td>Vidya Malvade</td>
      <td>Sagarika Ghatge</td>
      <td>Shilpa Shukla</td>
      <td>74129</td>
      <td>1113541</td>
    </tr>
    <tr>
      <th>149</th>
      <td>There Will Be Blood</td>
      <td>2007</td>
      <td>A</td>
      <td>158</td>
      <td>Drama</td>
      <td>8.2</td>
      <td>A story of family, religion, hatred, oil and m...</td>
      <td>93.00000</td>
      <td>Paul Thomas Anderson</td>
      <td>Daniel Day-Lewis</td>
      <td>Paul Dano</td>
      <td>Ciarán Hinds</td>
      <td>Martin Stringer</td>
      <td>517359</td>
      <td>40222514</td>
    </tr>
    <tr>
      <th>150</th>
      <td>Pan's Labyrinth</td>
      <td>2006</td>
      <td>UA</td>
      <td>118</td>
      <td>Drama, Fantasy, War</td>
      <td>8.2</td>
      <td>In the Falangist Spain of 1944, the bookish yo...</td>
      <td>98.00000</td>
      <td>Guillermo del Toro</td>
      <td>Ivana Baquero</td>
      <td>Ariadna Gil</td>
      <td>Sergi López</td>
      <td>Maribel Verdú</td>
      <td>618623</td>
      <td>37634615</td>
    </tr>
    <tr>
      <th>151</th>
      <td>Toy Story 3</td>
      <td>2010</td>
      <td>U</td>
      <td>103</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.2</td>
      <td>The toys are mistakenly delivered to a day-car...</td>
      <td>92.00000</td>
      <td>Lee Unkrich</td>
      <td>Tom Hanks</td>
      <td>Tim Allen</td>
      <td>Joan Cusack</td>
      <td>Ned Beatty</td>
      <td>757032</td>
      <td>415004880</td>
    </tr>
    <tr>
      <th>152</th>
      <td>V for Vendetta</td>
      <td>2005</td>
      <td>A</td>
      <td>132</td>
      <td>Action, Drama, Sci-Fi</td>
      <td>8.2</td>
      <td>In a future British tyranny, a shadowy freedom...</td>
      <td>62.00000</td>
      <td>James McTeigue</td>
      <td>Hugo Weaving</td>
      <td>Natalie Portman</td>
      <td>Rupert Graves</td>
      <td>Stephen Rea</td>
      <td>1032749</td>
      <td>70511035</td>
    </tr>
    <tr>
      <th>153</th>
      <td>Rang De Basanti</td>
      <td>2006</td>
      <td>UA</td>
      <td>167</td>
      <td>Comedy, Crime, Drama</td>
      <td>8.2</td>
      <td>The story of six young Indians who assist an E...</td>
      <td>77.97153</td>
      <td>Rakeysh Omprakash Mehra</td>
      <td>Aamir Khan</td>
      <td>Soha Ali Khan</td>
      <td>Siddharth</td>
      <td>Sharman Joshi</td>
      <td>111937</td>
      <td>2197331</td>
    </tr>
    <tr>
      <th>154</th>
      <td>Black</td>
      <td>2005</td>
      <td>U</td>
      <td>122</td>
      <td>Drama</td>
      <td>8.2</td>
      <td>The cathartic tale of a young woman who can't ...</td>
      <td>77.97153</td>
      <td>Sanjay Leela Bhansali</td>
      <td>Amitabh Bachchan</td>
      <td>Rani Mukerji</td>
      <td>Shernaz Patel</td>
      <td>Ayesha Kapoor</td>
      <td>33354</td>
      <td>733094</td>
    </tr>
    <tr>
      <th>155</th>
      <td>Batman Begins</td>
      <td>2005</td>
      <td>UA</td>
      <td>140</td>
      <td>Action, Adventure</td>
      <td>8.2</td>
      <td>After training with his mentor, Batman begins ...</td>
      <td>70.00000</td>
      <td>Christopher Nolan</td>
      <td>Christian Bale</td>
      <td>Michael Caine</td>
      <td>Ken Watanabe</td>
      <td>Liam Neeson</td>
      <td>1308302</td>
      <td>206852432</td>
    </tr>
    <tr>
      <th>156</th>
      <td>Swades: We, the People</td>
      <td>2004</td>
      <td>U</td>
      <td>210</td>
      <td>Drama</td>
      <td>8.2</td>
      <td>A successful Indian scientist returns to an In...</td>
      <td>77.97153</td>
      <td>Ashutosh Gowariker</td>
      <td>Shah Rukh Khan</td>
      <td>Gayatri Joshi</td>
      <td>Kishori Ballal</td>
      <td>Smit Sheth</td>
      <td>83005</td>
      <td>1223240</td>
    </tr>
    <tr>
      <th>157</th>
      <td>Der Untergang</td>
      <td>2004</td>
      <td>R</td>
      <td>156</td>
      <td>Biography, Drama, History</td>
      <td>8.2</td>
      <td>Traudl Junge, the final secretary for Adolf Hi...</td>
      <td>82.00000</td>
      <td>Oliver Hirschbiegel</td>
      <td>Bruno Ganz</td>
      <td>Alexandra Maria Lara</td>
      <td>Ulrich Matthes</td>
      <td>Juliane Köhler</td>
      <td>331308</td>
      <td>5509040</td>
    </tr>
    <tr>
      <th>158</th>
      <td>Hauru no ugoku shiro</td>
      <td>2004</td>
      <td>U</td>
      <td>119</td>
      <td>Animation, Adventure, Family</td>
      <td>8.2</td>
      <td>When an unconfident young woman is cursed with...</td>
      <td>80.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Chieko Baishô</td>
      <td>Takuya Kimura</td>
      <td>Tatsuya Gashûin</td>
      <td>Akihiro Miwa</td>
      <td>333915</td>
      <td>4711096</td>
    </tr>
    <tr>
      <th>159</th>
      <td>A Beautiful Mind</td>
      <td>2001</td>
      <td>UA</td>
      <td>135</td>
      <td>Biography, Drama</td>
      <td>8.2</td>
      <td>After John Nash, a brilliant but asocial mathe...</td>
      <td>72.00000</td>
      <td>Ron Howard</td>
      <td>Russell Crowe</td>
      <td>Ed Harris</td>
      <td>Jennifer Connelly</td>
      <td>Christopher Plummer</td>
      <td>848920</td>
      <td>170742341</td>
    </tr>
    <tr>
      <th>160</th>
      <td>Hera Pheri</td>
      <td>2000</td>
      <td>U</td>
      <td>156</td>
      <td>Action, Comedy, Crime</td>
      <td>8.2</td>
      <td>Three unemployed men look for answers to all t...</td>
      <td>77.97153</td>
      <td>Priyadarshan</td>
      <td>Akshay Kumar</td>
      <td>Sunil Shetty</td>
      <td>Paresh Rawal</td>
      <td>Tabu</td>
      <td>57057</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>161</th>
      <td>Lock, Stock and Two Smoking Barrels</td>
      <td>1998</td>
      <td>A</td>
      <td>107</td>
      <td>Action, Comedy, Crime</td>
      <td>8.2</td>
      <td>A botched card game in London triggers four fr...</td>
      <td>66.00000</td>
      <td>Guy Ritchie</td>
      <td>Jason Flemyng</td>
      <td>Dexter Fletcher</td>
      <td>Nick Moran</td>
      <td>Jason Statham</td>
      <td>535216</td>
      <td>3897569</td>
    </tr>
    <tr>
      <th>162</th>
      <td>L.A. Confidential</td>
      <td>1997</td>
      <td>A</td>
      <td>138</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.2</td>
      <td>As corruption grows in 1950s Los Angeles, thre...</td>
      <td>90.00000</td>
      <td>Curtis Hanson</td>
      <td>Kevin Spacey</td>
      <td>Russell Crowe</td>
      <td>Guy Pearce</td>
      <td>Kim Basinger</td>
      <td>531967</td>
      <td>64616940</td>
    </tr>
    <tr>
      <th>163</th>
      <td>Eskiya</td>
      <td>1996</td>
      <td>Unknown</td>
      <td>128</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.2</td>
      <td>Baran the Bandit, released from prison after 3...</td>
      <td>77.97153</td>
      <td>Yavuz Turgul</td>
      <td>Sener Sen</td>
      <td>Ugur Yücel</td>
      <td>Sermin Hürmeriç</td>
      <td>Yesim Salkim</td>
      <td>64118</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>164</th>
      <td>Heat</td>
      <td>1995</td>
      <td>A</td>
      <td>170</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.2</td>
      <td>A group of professional bank robbers start to ...</td>
      <td>76.00000</td>
      <td>Michael Mann</td>
      <td>Al Pacino</td>
      <td>Robert De Niro</td>
      <td>Val Kilmer</td>
      <td>Jon Voight</td>
      <td>577113</td>
      <td>67436818</td>
    </tr>
    <tr>
      <th>165</th>
      <td>Casino</td>
      <td>1995</td>
      <td>A</td>
      <td>178</td>
      <td>Crime, Drama</td>
      <td>8.2</td>
      <td>A tale of greed, deception, money, power, and ...</td>
      <td>73.00000</td>
      <td>Martin Scorsese</td>
      <td>Robert De Niro</td>
      <td>Sharon Stone</td>
      <td>Joe Pesci</td>
      <td>James Woods</td>
      <td>466276</td>
      <td>42438300</td>
    </tr>
    <tr>
      <th>166</th>
      <td>Andaz Apna Apna</td>
      <td>1994</td>
      <td>U</td>
      <td>160</td>
      <td>Action, Comedy, Romance</td>
      <td>8.2</td>
      <td>Two slackers competing for the affections of a...</td>
      <td>77.97153</td>
      <td>Rajkumar Santoshi</td>
      <td>Aamir Khan</td>
      <td>Salman Khan</td>
      <td>Raveena Tandon</td>
      <td>Karisma Kapoor</td>
      <td>49300</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>167</th>
      <td>Unforgiven</td>
      <td>1992</td>
      <td>A</td>
      <td>130</td>
      <td>Drama, Western</td>
      <td>8.2</td>
      <td>Retired Old West gunslinger William Munny relu...</td>
      <td>85.00000</td>
      <td>Clint Eastwood</td>
      <td>Clint Eastwood</td>
      <td>Gene Hackman</td>
      <td>Morgan Freeman</td>
      <td>Richard Harris</td>
      <td>375935</td>
      <td>101157447</td>
    </tr>
    <tr>
      <th>168</th>
      <td>Indiana Jones and the Last Crusade</td>
      <td>1989</td>
      <td>U</td>
      <td>127</td>
      <td>Action, Adventure</td>
      <td>8.2</td>
      <td>In 1938, after his father Professor Henry Jone...</td>
      <td>65.00000</td>
      <td>Steven Spielberg</td>
      <td>Harrison Ford</td>
      <td>Sean Connery</td>
      <td>Alison Doody</td>
      <td>Denholm Elliott</td>
      <td>692366</td>
      <td>197171806</td>
    </tr>
    <tr>
      <th>169</th>
      <td>Dom za vesanje</td>
      <td>1988</td>
      <td>R</td>
      <td>142</td>
      <td>Comedy, Crime, Drama</td>
      <td>8.2</td>
      <td>In this luminous tale set in the area around S...</td>
      <td>77.97153</td>
      <td>Emir Kusturica</td>
      <td>Davor Dujmovic</td>
      <td>Bora Todorovic</td>
      <td>Ljubica Adzovic</td>
      <td>Husnija Hasimovic</td>
      <td>26402</td>
      <td>280015</td>
    </tr>
    <tr>
      <th>170</th>
      <td>Tonari no Totoro</td>
      <td>1988</td>
      <td>U</td>
      <td>86</td>
      <td>Animation, Family, Fantasy</td>
      <td>8.2</td>
      <td>When two girls move to the country to be near ...</td>
      <td>86.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Hitoshi Takagi</td>
      <td>Noriko Hidaka</td>
      <td>Chika Sakamoto</td>
      <td>Shigesato Itoi</td>
      <td>291180</td>
      <td>1105564</td>
    </tr>
    <tr>
      <th>171</th>
      <td>Die Hard</td>
      <td>1988</td>
      <td>A</td>
      <td>132</td>
      <td>Action, Thriller</td>
      <td>8.2</td>
      <td>An NYPD officer tries to save his wife and sev...</td>
      <td>72.00000</td>
      <td>John McTiernan</td>
      <td>Bruce Willis</td>
      <td>Alan Rickman</td>
      <td>Bonnie Bedelia</td>
      <td>Reginald VelJohnson</td>
      <td>793164</td>
      <td>83008852</td>
    </tr>
    <tr>
      <th>172</th>
      <td>Ran</td>
      <td>1985</td>
      <td>U</td>
      <td>162</td>
      <td>Action, Drama, War</td>
      <td>8.2</td>
      <td>In Medieval Japan, an elderly warlord retires,...</td>
      <td>96.00000</td>
      <td>Akira Kurosawa</td>
      <td>Tatsuya Nakadai</td>
      <td>Akira Terao</td>
      <td>Jinpachi Nezu</td>
      <td>Daisuke Ryû</td>
      <td>112505</td>
      <td>4135750</td>
    </tr>
    <tr>
      <th>173</th>
      <td>Raging Bull</td>
      <td>1980</td>
      <td>A</td>
      <td>129</td>
      <td>Biography, Drama, Sport</td>
      <td>8.2</td>
      <td>The life of boxer Jake LaMotta, whose violence...</td>
      <td>89.00000</td>
      <td>Martin Scorsese</td>
      <td>Robert De Niro</td>
      <td>Cathy Moriarty</td>
      <td>Joe Pesci</td>
      <td>Frank Vincent</td>
      <td>321860</td>
      <td>23383987</td>
    </tr>
    <tr>
      <th>174</th>
      <td>Stalker</td>
      <td>1979</td>
      <td>U</td>
      <td>162</td>
      <td>Drama, Sci-Fi</td>
      <td>8.2</td>
      <td>A guide leads two men through an area known as...</td>
      <td>77.97153</td>
      <td>Andrei Tarkovsky</td>
      <td>Alisa Freyndlikh</td>
      <td>Aleksandr Kaydanovskiy</td>
      <td>Anatoliy Solonitsyn</td>
      <td>Nikolay Grinko</td>
      <td>116945</td>
      <td>234723</td>
    </tr>
    <tr>
      <th>175</th>
      <td>Höstsonaten</td>
      <td>1978</td>
      <td>U</td>
      <td>99</td>
      <td>Drama, Music</td>
      <td>8.2</td>
      <td>A married daughter who longs for her mother's ...</td>
      <td>77.97153</td>
      <td>Ingmar Bergman</td>
      <td>Ingrid Bergman</td>
      <td>Liv Ullmann</td>
      <td>Lena Nyman</td>
      <td>Halvar Björk</td>
      <td>26875</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>176</th>
      <td>The Message</td>
      <td>1976</td>
      <td>PG</td>
      <td>177</td>
      <td>Biography, Drama, History</td>
      <td>8.2</td>
      <td>This epic historical drama chronicles the life...</td>
      <td>77.97153</td>
      <td>Moustapha Akkad</td>
      <td>Anthony Quinn</td>
      <td>Irene Papas</td>
      <td>Michael Ansara</td>
      <td>Johnny Sekka</td>
      <td>43885</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>177</th>
      <td>Sholay</td>
      <td>1975</td>
      <td>U</td>
      <td>204</td>
      <td>Action, Adventure, Comedy</td>
      <td>8.2</td>
      <td>After his family is murdered by a notorious an...</td>
      <td>77.97153</td>
      <td>Ramesh Sippy</td>
      <td>Sanjeev Kumar</td>
      <td>Dharmendra</td>
      <td>Amitabh Bachchan</td>
      <td>Amjad Khan</td>
      <td>51284</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>178</th>
      <td>Monty Python and the Holy Grail</td>
      <td>1975</td>
      <td>PG</td>
      <td>91</td>
      <td>Adventure, Comedy, Fantasy</td>
      <td>8.2</td>
      <td>King Arthur and his Knights of the Round Table...</td>
      <td>91.00000</td>
      <td>Terry Gilliam</td>
      <td>Terry Jones</td>
      <td>Graham Chapman</td>
      <td>John Cleese</td>
      <td>Eric Idle</td>
      <td>500875</td>
      <td>1229197</td>
    </tr>
    <tr>
      <th>179</th>
      <td>The Great Escape</td>
      <td>1963</td>
      <td>U</td>
      <td>172</td>
      <td>Adventure, Drama, History</td>
      <td>8.2</td>
      <td>Allied prisoners of war plan for several hundr...</td>
      <td>86.00000</td>
      <td>John Sturges</td>
      <td>Steve McQueen</td>
      <td>James Garner</td>
      <td>Richard Attenborough</td>
      <td>Charles Bronson</td>
      <td>224730</td>
      <td>12100000</td>
    </tr>
    <tr>
      <th>180</th>
      <td>To Kill a Mockingbird</td>
      <td>1962</td>
      <td>U</td>
      <td>129</td>
      <td>Crime, Drama</td>
      <td>8.2</td>
      <td>Atticus Finch, a lawyer in the Depression-era ...</td>
      <td>88.00000</td>
      <td>Robert Mulligan</td>
      <td>Gregory Peck</td>
      <td>John Megna</td>
      <td>Frank Overton</td>
      <td>Rosemary Murphy</td>
      <td>293811</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>181</th>
      <td>Yôjinbô</td>
      <td>1961</td>
      <td>Unknown</td>
      <td>110</td>
      <td>Action, Drama, Thriller</td>
      <td>8.2</td>
      <td>A crafty ronin comes to a town divided by two ...</td>
      <td>77.97153</td>
      <td>Akira Kurosawa</td>
      <td>Toshirô Mifune</td>
      <td>Eijirô Tôno</td>
      <td>Tatsuya Nakadai</td>
      <td>Yôko Tsukasa</td>
      <td>111244</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>182</th>
      <td>Judgment at Nuremberg</td>
      <td>1961</td>
      <td>A</td>
      <td>179</td>
      <td>Drama, War</td>
      <td>8.2</td>
      <td>In 1948, an American court in occupied Germany...</td>
      <td>60.00000</td>
      <td>Stanley Kramer</td>
      <td>Spencer Tracy</td>
      <td>Burt Lancaster</td>
      <td>Richard Widmark</td>
      <td>Marlene Dietrich</td>
      <td>69458</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>183</th>
      <td>Some Like It Hot</td>
      <td>1959</td>
      <td>U</td>
      <td>121</td>
      <td>Comedy, Music, Romance</td>
      <td>8.2</td>
      <td>After two male musicians witness a mob hit, th...</td>
      <td>98.00000</td>
      <td>Billy Wilder</td>
      <td>Marilyn Monroe</td>
      <td>Tony Curtis</td>
      <td>Jack Lemmon</td>
      <td>George Raft</td>
      <td>243943</td>
      <td>25000000</td>
    </tr>
    <tr>
      <th>184</th>
      <td>Smultronstället</td>
      <td>1957</td>
      <td>U</td>
      <td>91</td>
      <td>Drama, Romance</td>
      <td>8.2</td>
      <td>After living a life marked by coldness, an agi...</td>
      <td>88.00000</td>
      <td>Ingmar Bergman</td>
      <td>Victor Sjöström</td>
      <td>Bibi Andersson</td>
      <td>Ingrid Thulin</td>
      <td>Gunnar Björnstrand</td>
      <td>96381</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>185</th>
      <td>Det sjunde inseglet</td>
      <td>1957</td>
      <td>A</td>
      <td>96</td>
      <td>Drama, Fantasy, History</td>
      <td>8.2</td>
      <td>A man seeks answers about life, death, and the...</td>
      <td>88.00000</td>
      <td>Ingmar Bergman</td>
      <td>Max von Sydow</td>
      <td>Gunnar Björnstrand</td>
      <td>Bengt Ekerot</td>
      <td>Nils Poppe</td>
      <td>164939</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>186</th>
      <td>Du rififi chez les hommes</td>
      <td>1955</td>
      <td>Unknown</td>
      <td>118</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.2</td>
      <td>Four men plan a technically perfect crime, but...</td>
      <td>97.00000</td>
      <td>Jules Dassin</td>
      <td>Jean Servais</td>
      <td>Carl Möhner</td>
      <td>Robert Manuel</td>
      <td>Janine Darcey</td>
      <td>28810</td>
      <td>57226</td>
    </tr>
    <tr>
      <th>187</th>
      <td>Dial M for Murder</td>
      <td>1954</td>
      <td>A</td>
      <td>105</td>
      <td>Crime, Thriller</td>
      <td>8.2</td>
      <td>A former tennis player tries to arrange his wi...</td>
      <td>75.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Ray Milland</td>
      <td>Grace Kelly</td>
      <td>Robert Cummings</td>
      <td>John Williams</td>
      <td>158335</td>
      <td>12562</td>
    </tr>
    <tr>
      <th>188</th>
      <td>Tôkyô monogatari</td>
      <td>1953</td>
      <td>U</td>
      <td>136</td>
      <td>Drama</td>
      <td>8.2</td>
      <td>An old couple visit their children and grandch...</td>
      <td>77.97153</td>
      <td>Yasujirô Ozu</td>
      <td>Chishû Ryû</td>
      <td>Chieko Higashiyama</td>
      <td>Sô Yamamura</td>
      <td>Setsuko Hara</td>
      <td>53153</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>189</th>
      <td>Rashômon</td>
      <td>1950</td>
      <td>Unknown</td>
      <td>88</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.2</td>
      <td>The rape of a bride and the murder of her samu...</td>
      <td>98.00000</td>
      <td>Akira Kurosawa</td>
      <td>Toshirô Mifune</td>
      <td>Machiko Kyô</td>
      <td>Masayuki Mori</td>
      <td>Takashi Shimura</td>
      <td>152572</td>
      <td>96568</td>
    </tr>
    <tr>
      <th>190</th>
      <td>All About Eve</td>
      <td>1950</td>
      <td>Passed</td>
      <td>138</td>
      <td>Drama</td>
      <td>8.2</td>
      <td>A seemingly timid but secretly ruthless ingénu...</td>
      <td>98.00000</td>
      <td>Joseph L. Mankiewicz</td>
      <td>Bette Davis</td>
      <td>Anne Baxter</td>
      <td>George Sanders</td>
      <td>Celeste Holm</td>
      <td>120539</td>
      <td>10177</td>
    </tr>
    <tr>
      <th>191</th>
      <td>The Treasure of the Sierra Madre</td>
      <td>1948</td>
      <td>Passed</td>
      <td>126</td>
      <td>Adventure, Drama, Western</td>
      <td>8.2</td>
      <td>Two Americans searching for work in Mexico con...</td>
      <td>98.00000</td>
      <td>John Huston</td>
      <td>Humphrey Bogart</td>
      <td>Walter Huston</td>
      <td>Tim Holt</td>
      <td>Bruce Bennett</td>
      <td>114304</td>
      <td>5014000</td>
    </tr>
    <tr>
      <th>192</th>
      <td>To Be or Not to Be</td>
      <td>1942</td>
      <td>Passed</td>
      <td>99</td>
      <td>Comedy, War</td>
      <td>8.2</td>
      <td>During the Nazi occupation of Poland, an actin...</td>
      <td>86.00000</td>
      <td>Ernst Lubitsch</td>
      <td>Carole Lombard</td>
      <td>Jack Benny</td>
      <td>Robert Stack</td>
      <td>Felix Bressart</td>
      <td>29915</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>193</th>
      <td>The Gold Rush</td>
      <td>1925</td>
      <td>Passed</td>
      <td>95</td>
      <td>Adventure, Comedy, Drama</td>
      <td>8.2</td>
      <td>A prospector goes to the Klondike in search of...</td>
      <td>77.97153</td>
      <td>Charles Chaplin</td>
      <td>Charles Chaplin</td>
      <td>Mack Swain</td>
      <td>Tom Murray</td>
      <td>Henry Bergman</td>
      <td>101053</td>
      <td>5450000</td>
    </tr>
    <tr>
      <th>194</th>
      <td>Sherlock Jr.</td>
      <td>1924</td>
      <td>Passed</td>
      <td>45</td>
      <td>Action, Comedy, Romance</td>
      <td>8.2</td>
      <td>A film projectionist longs to be a detective, ...</td>
      <td>77.97153</td>
      <td>Buster Keaton</td>
      <td>Buster Keaton</td>
      <td>Kathryn McGuire</td>
      <td>Joe Keaton</td>
      <td>Erwin Connelly</td>
      <td>41985</td>
      <td>977375</td>
    </tr>
    <tr>
      <th>195</th>
      <td>Portrait de la jeune fille en feu</td>
      <td>2019</td>
      <td>R</td>
      <td>122</td>
      <td>Drama, Romance</td>
      <td>8.1</td>
      <td>On an isolated island in Brittany at the end o...</td>
      <td>95.00000</td>
      <td>Céline Sciamma</td>
      <td>Noémie Merlant</td>
      <td>Adèle Haenel</td>
      <td>Luàna Bajrami</td>
      <td>Valeria Golino</td>
      <td>63134</td>
      <td>3759854</td>
    </tr>
    <tr>
      <th>196</th>
      <td>Pink</td>
      <td>2016</td>
      <td>UA</td>
      <td>136</td>
      <td>Drama, Thriller</td>
      <td>8.1</td>
      <td>When three young women are implicated in a cri...</td>
      <td>77.97153</td>
      <td>Aniruddha Roy Chowdhury</td>
      <td>Taapsee Pannu</td>
      <td>Amitabh Bachchan</td>
      <td>Kirti Kulhari</td>
      <td>Andrea Tariang</td>
      <td>39216</td>
      <td>1241223</td>
    </tr>
    <tr>
      <th>197</th>
      <td>Koe no katachi</td>
      <td>2016</td>
      <td>16</td>
      <td>130</td>
      <td>Animation, Drama, Family</td>
      <td>8.1</td>
      <td>A young man is ostracized by his classmates af...</td>
      <td>78.00000</td>
      <td>Naoko Yamada</td>
      <td>Miyu Irino</td>
      <td>Saori Hayami</td>
      <td>Aoi Yûki</td>
      <td>Kenshô Ono</td>
      <td>47708</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>198</th>
      <td>Contratiempo</td>
      <td>2016</td>
      <td>TV-MA</td>
      <td>106</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.1</td>
      <td>A successful entrepreneur accused of murder an...</td>
      <td>77.97153</td>
      <td>Oriol Paulo</td>
      <td>Mario Casas</td>
      <td>Ana Wagener</td>
      <td>Jose Coronado</td>
      <td>Bárbara Lennie</td>
      <td>141516</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>199</th>
      <td>Ah-ga-ssi</td>
      <td>2016</td>
      <td>A</td>
      <td>145</td>
      <td>Drama, Romance, Thriller</td>
      <td>8.1</td>
      <td>A woman is hired as a handmaiden to a Japanese...</td>
      <td>84.00000</td>
      <td>Chan-wook Park</td>
      <td>Kim Min-hee</td>
      <td>Jung-woo Ha</td>
      <td>Cho Jin-woong</td>
      <td>Moon So-Ri</td>
      <td>113649</td>
      <td>2006788</td>
    </tr>
    <tr>
      <th>200</th>
      <td>Mommy</td>
      <td>2014</td>
      <td>R</td>
      <td>139</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>A widowed single mother, raising her violent s...</td>
      <td>74.00000</td>
      <td>Xavier Dolan</td>
      <td>Anne Dorval</td>
      <td>Antoine Olivier Pilon</td>
      <td>Suzanne Clément</td>
      <td>Patrick Huard</td>
      <td>50700</td>
      <td>3492754</td>
    </tr>
    <tr>
      <th>201</th>
      <td>Haider</td>
      <td>2014</td>
      <td>UA</td>
      <td>160</td>
      <td>Action, Crime, Drama</td>
      <td>8.1</td>
      <td>A young man returns to Kashmir after his fathe...</td>
      <td>77.97153</td>
      <td>Vishal Bhardwaj</td>
      <td>Shahid Kapoor</td>
      <td>Tabu</td>
      <td>Shraddha Kapoor</td>
      <td>Kay Kay Menon</td>
      <td>50445</td>
      <td>901610</td>
    </tr>
    <tr>
      <th>202</th>
      <td>Logan</td>
      <td>2017</td>
      <td>A</td>
      <td>137</td>
      <td>Action, Drama, Sci-Fi</td>
      <td>8.1</td>
      <td>In a future where mutants are nearly extinct, ...</td>
      <td>77.00000</td>
      <td>James Mangold</td>
      <td>Hugh Jackman</td>
      <td>Patrick Stewart</td>
      <td>Dafne Keen</td>
      <td>Boyd Holbrook</td>
      <td>647884</td>
      <td>226277068</td>
    </tr>
    <tr>
      <th>203</th>
      <td>Room</td>
      <td>2015</td>
      <td>R</td>
      <td>118</td>
      <td>Drama, Thriller</td>
      <td>8.1</td>
      <td>Held captive for 7 years in an enclosed space,...</td>
      <td>86.00000</td>
      <td>Lenny Abrahamson</td>
      <td>Brie Larson</td>
      <td>Jacob Tremblay</td>
      <td>Sean Bridgers</td>
      <td>Wendy Crewson</td>
      <td>371538</td>
      <td>14677674</td>
    </tr>
    <tr>
      <th>204</th>
      <td>Relatos salvajes</td>
      <td>2014</td>
      <td>R</td>
      <td>122</td>
      <td>Comedy, Drama, Thriller</td>
      <td>8.1</td>
      <td>Six short stories that explore the extremities...</td>
      <td>77.00000</td>
      <td>Damián Szifron</td>
      <td>Darío Grandinetti</td>
      <td>María Marull</td>
      <td>Mónica Villa</td>
      <td>Diego Starosta</td>
      <td>177059</td>
      <td>3107072</td>
    </tr>
    <tr>
      <th>205</th>
      <td>Soul</td>
      <td>2020</td>
      <td>U</td>
      <td>100</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.1</td>
      <td>After landing the gig of a lifetime, a New Yor...</td>
      <td>83.00000</td>
      <td>Pete Docter</td>
      <td>Kemp Powers</td>
      <td>Jamie Foxx</td>
      <td>Tina Fey</td>
      <td>Graham Norton</td>
      <td>159171</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>206</th>
      <td>Kis Uykusu</td>
      <td>2014</td>
      <td>Unknown</td>
      <td>196</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>A hotel owner and landlord in a remote Turkish...</td>
      <td>88.00000</td>
      <td>Nuri Bilge Ceylan</td>
      <td>Haluk Bilginer</td>
      <td>Melisa Sözen</td>
      <td>Demet Akbag</td>
      <td>Ayberk Pekcan</td>
      <td>46547</td>
      <td>165520</td>
    </tr>
    <tr>
      <th>207</th>
      <td>PK</td>
      <td>2014</td>
      <td>UA</td>
      <td>153</td>
      <td>Comedy, Drama, Musical</td>
      <td>8.1</td>
      <td>An alien on Earth loses the only device he can...</td>
      <td>77.97153</td>
      <td>Rajkumar Hirani</td>
      <td>Aamir Khan</td>
      <td>Anushka Sharma</td>
      <td>Sanjay Dutt</td>
      <td>Boman Irani</td>
      <td>163061</td>
      <td>10616104</td>
    </tr>
    <tr>
      <th>208</th>
      <td>OMG: Oh My God!</td>
      <td>2012</td>
      <td>U</td>
      <td>125</td>
      <td>Comedy, Drama, Fantasy</td>
      <td>8.1</td>
      <td>A shopkeeper takes God to court when his shop ...</td>
      <td>77.97153</td>
      <td>Umesh Shukla</td>
      <td>Paresh Rawal</td>
      <td>Akshay Kumar</td>
      <td>Mithun Chakraborty</td>
      <td>Mahesh Manjrekar</td>
      <td>51739</td>
      <td>923221</td>
    </tr>
    <tr>
      <th>209</th>
      <td>The Grand Budapest Hotel</td>
      <td>2014</td>
      <td>UA</td>
      <td>99</td>
      <td>Adventure, Comedy, Crime</td>
      <td>8.1</td>
      <td>A writer encounters the owner of an aging high...</td>
      <td>88.00000</td>
      <td>Wes Anderson</td>
      <td>Ralph Fiennes</td>
      <td>F. Murray Abraham</td>
      <td>Mathieu Amalric</td>
      <td>Adrien Brody</td>
      <td>707630</td>
      <td>59100318</td>
    </tr>
    <tr>
      <th>210</th>
      <td>Gone Girl</td>
      <td>2014</td>
      <td>A</td>
      <td>149</td>
      <td>Drama, Mystery, Thriller</td>
      <td>8.1</td>
      <td>With his wife's disappearance having become th...</td>
      <td>79.00000</td>
      <td>David Fincher</td>
      <td>Ben Affleck</td>
      <td>Rosamund Pike</td>
      <td>Neil Patrick Harris</td>
      <td>Tyler Perry</td>
      <td>859695</td>
      <td>167767189</td>
    </tr>
    <tr>
      <th>211</th>
      <td>Ôkami kodomo no Ame to Yuki</td>
      <td>2012</td>
      <td>U</td>
      <td>117</td>
      <td>Animation, Drama, Fantasy</td>
      <td>8.1</td>
      <td>After her werewolf lover unexpectedly dies in ...</td>
      <td>71.00000</td>
      <td>Mamoru Hosoda</td>
      <td>Aoi Miyazaki</td>
      <td>Takao Osawa</td>
      <td>Haru Kuroki</td>
      <td>Yukito Nishii</td>
      <td>38803</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>212</th>
      <td>Hacksaw Ridge</td>
      <td>2016</td>
      <td>A</td>
      <td>139</td>
      <td>Biography, Drama, History</td>
      <td>8.1</td>
      <td>World War II American Army Medic Desmond T. Do...</td>
      <td>71.00000</td>
      <td>Mel Gibson</td>
      <td>Andrew Garfield</td>
      <td>Sam Worthington</td>
      <td>Luke Bracey</td>
      <td>Teresa Palmer</td>
      <td>435928</td>
      <td>67209615</td>
    </tr>
    <tr>
      <th>213</th>
      <td>Inside Out</td>
      <td>2015</td>
      <td>U</td>
      <td>95</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.1</td>
      <td>After young Riley is uprooted from her Midwest...</td>
      <td>94.00000</td>
      <td>Pete Docter</td>
      <td>Ronnie Del Carmen</td>
      <td>Amy Poehler</td>
      <td>Bill Hader</td>
      <td>Lewis Black</td>
      <td>616228</td>
      <td>356461711</td>
    </tr>
    <tr>
      <th>214</th>
      <td>Barfi!</td>
      <td>2012</td>
      <td>U</td>
      <td>151</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.1</td>
      <td>Three young people learn that love can neither...</td>
      <td>77.97153</td>
      <td>Anurag Basu</td>
      <td>Ranbir Kapoor</td>
      <td>Priyanka Chopra</td>
      <td>Ileana D'Cruz</td>
      <td>Saurabh Shukla</td>
      <td>75721</td>
      <td>2804874</td>
    </tr>
    <tr>
      <th>215</th>
      <td>12 Years a Slave</td>
      <td>2013</td>
      <td>A</td>
      <td>134</td>
      <td>Biography, Drama, History</td>
      <td>8.1</td>
      <td>In the antebellum United States, Solomon North...</td>
      <td>96.00000</td>
      <td>Steve McQueen</td>
      <td>Chiwetel Ejiofor</td>
      <td>Michael Kenneth Williams</td>
      <td>Michael Fassbender</td>
      <td>Brad Pitt</td>
      <td>640533</td>
      <td>56671993</td>
    </tr>
    <tr>
      <th>216</th>
      <td>Rush</td>
      <td>2013</td>
      <td>UA</td>
      <td>123</td>
      <td>Action, Biography, Drama</td>
      <td>8.1</td>
      <td>The merciless 1970s rivalry between Formula On...</td>
      <td>74.00000</td>
      <td>Ron Howard</td>
      <td>Daniel Brühl</td>
      <td>Chris Hemsworth</td>
      <td>Olivia Wilde</td>
      <td>Alexandra Maria Lara</td>
      <td>432811</td>
      <td>26947624</td>
    </tr>
    <tr>
      <th>217</th>
      <td>Ford v Ferrari</td>
      <td>2019</td>
      <td>UA</td>
      <td>152</td>
      <td>Action, Biography, Drama</td>
      <td>8.1</td>
      <td>American car designer Carroll Shelby and drive...</td>
      <td>81.00000</td>
      <td>James Mangold</td>
      <td>Matt Damon</td>
      <td>Christian Bale</td>
      <td>Jon Bernthal</td>
      <td>Caitriona Balfe</td>
      <td>291289</td>
      <td>117624028</td>
    </tr>
    <tr>
      <th>218</th>
      <td>Spotlight</td>
      <td>2015</td>
      <td>A</td>
      <td>129</td>
      <td>Biography, Crime, Drama</td>
      <td>8.1</td>
      <td>The true story of how the Boston Globe uncover...</td>
      <td>93.00000</td>
      <td>Tom McCarthy</td>
      <td>Mark Ruffalo</td>
      <td>Michael Keaton</td>
      <td>Rachel McAdams</td>
      <td>Liev Schreiber</td>
      <td>420316</td>
      <td>45055776</td>
    </tr>
    <tr>
      <th>219</th>
      <td>Song of the Sea</td>
      <td>2014</td>
      <td>PG</td>
      <td>93</td>
      <td>Animation, Adventure, Drama</td>
      <td>8.1</td>
      <td>Ben, a young Irish boy, and his little sister ...</td>
      <td>85.00000</td>
      <td>Tomm Moore</td>
      <td>David Rawle</td>
      <td>Brendan Gleeson</td>
      <td>Lisa Hannigan</td>
      <td>Fionnula Flanagan</td>
      <td>51679</td>
      <td>857524</td>
    </tr>
    <tr>
      <th>220</th>
      <td>Kahaani</td>
      <td>2012</td>
      <td>UA</td>
      <td>122</td>
      <td>Mystery, Thriller</td>
      <td>8.1</td>
      <td>A pregnant woman's search for her missing husb...</td>
      <td>77.97153</td>
      <td>Sujoy Ghosh</td>
      <td>Vidya Balan</td>
      <td>Parambrata Chattopadhyay</td>
      <td>Indraneil Sengupta</td>
      <td>Nawazuddin Siddiqui</td>
      <td>57806</td>
      <td>1035953</td>
    </tr>
    <tr>
      <th>221</th>
      <td>Zindagi Na Milegi Dobara</td>
      <td>2011</td>
      <td>U</td>
      <td>155</td>
      <td>Comedy, Drama</td>
      <td>8.1</td>
      <td>Three friends decide to turn their fantasy vac...</td>
      <td>77.97153</td>
      <td>Zoya Akhtar</td>
      <td>Hrithik Roshan</td>
      <td>Farhan Akhtar</td>
      <td>Abhay Deol</td>
      <td>Katrina Kaif</td>
      <td>67927</td>
      <td>3108485</td>
    </tr>
    <tr>
      <th>222</th>
      <td>Prisoners</td>
      <td>2013</td>
      <td>A</td>
      <td>153</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.1</td>
      <td>When Keller Dover's daughter and her friend go...</td>
      <td>70.00000</td>
      <td>Denis Villeneuve</td>
      <td>Hugh Jackman</td>
      <td>Jake Gyllenhaal</td>
      <td>Viola Davis</td>
      <td>Melissa Leo</td>
      <td>601149</td>
      <td>61002302</td>
    </tr>
    <tr>
      <th>223</th>
      <td>Mad Max: Fury Road</td>
      <td>2015</td>
      <td>UA</td>
      <td>120</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>8.1</td>
      <td>In a post-apocalyptic wasteland, a woman rebel...</td>
      <td>90.00000</td>
      <td>George Miller</td>
      <td>Tom Hardy</td>
      <td>Charlize Theron</td>
      <td>Nicholas Hoult</td>
      <td>Zoë Kravitz</td>
      <td>882316</td>
      <td>154058340</td>
    </tr>
    <tr>
      <th>224</th>
      <td>A Wednesday</td>
      <td>2008</td>
      <td>UA</td>
      <td>104</td>
      <td>Action, Crime, Drama</td>
      <td>8.1</td>
      <td>A retiring police officer reminisces about the...</td>
      <td>77.97153</td>
      <td>Neeraj Pandey</td>
      <td>Anupam Kher</td>
      <td>Naseeruddin Shah</td>
      <td>Jimmy Sheirgill</td>
      <td>Aamir Bashir</td>
      <td>73891</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>225</th>
      <td>Gran Torino</td>
      <td>2008</td>
      <td>R</td>
      <td>116</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>Disgruntled Korean War veteran Walt Kowalski s...</td>
      <td>72.00000</td>
      <td>Clint Eastwood</td>
      <td>Clint Eastwood</td>
      <td>Bee Vang</td>
      <td>Christopher Carley</td>
      <td>Ahney Her</td>
      <td>720450</td>
      <td>148095302</td>
    </tr>
    <tr>
      <th>226</th>
      <td>Harry Potter and the Deathly Hallows: Part 2</td>
      <td>2011</td>
      <td>UA</td>
      <td>130</td>
      <td>Adventure, Drama, Fantasy</td>
      <td>8.1</td>
      <td>Harry, Ron, and Hermione search for Voldemort'...</td>
      <td>85.00000</td>
      <td>David Yates</td>
      <td>Daniel Radcliffe</td>
      <td>Emma Watson</td>
      <td>Rupert Grint</td>
      <td>Michael Gambon</td>
      <td>764493</td>
      <td>381011219</td>
    </tr>
    <tr>
      <th>227</th>
      <td>Okuribito</td>
      <td>2008</td>
      <td>PG-13</td>
      <td>130</td>
      <td>Drama, Music</td>
      <td>8.1</td>
      <td>A newly unemployed cellist takes a job prepari...</td>
      <td>68.00000</td>
      <td>Yôjirô Takita</td>
      <td>Masahiro Motoki</td>
      <td>Ryôko Hirosue</td>
      <td>Tsutomu Yamazaki</td>
      <td>Kazuko Yoshiyuki</td>
      <td>48582</td>
      <td>1498210</td>
    </tr>
    <tr>
      <th>228</th>
      <td>Hachi: A Dog's Tale</td>
      <td>2009</td>
      <td>G</td>
      <td>93</td>
      <td>Biography, Drama, Family</td>
      <td>8.1</td>
      <td>A college professor bonds with an abandoned do...</td>
      <td>77.97153</td>
      <td>Lasse Hallström</td>
      <td>Richard Gere</td>
      <td>Joan Allen</td>
      <td>Cary-Hiroyuki Tagawa</td>
      <td>Sarah Roemer</td>
      <td>253575</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>229</th>
      <td>Mary and Max</td>
      <td>2009</td>
      <td>Unknown</td>
      <td>92</td>
      <td>Animation, Comedy, Drama</td>
      <td>8.1</td>
      <td>A tale of friendship between two unlikely pen ...</td>
      <td>77.97153</td>
      <td>Adam Elliot</td>
      <td>Toni Collette</td>
      <td>Philip Seymour Hoffman</td>
      <td>Eric Bana</td>
      <td>Barry Humphries</td>
      <td>164462</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>230</th>
      <td>How to Train Your Dragon</td>
      <td>2010</td>
      <td>U</td>
      <td>98</td>
      <td>Animation, Action, Adventure</td>
      <td>8.1</td>
      <td>A hapless young Viking who aspires to hunt dra...</td>
      <td>75.00000</td>
      <td>Dean DeBlois</td>
      <td>Chris Sanders</td>
      <td>Jay Baruchel</td>
      <td>Gerard Butler</td>
      <td>Christopher Mintz-Plasse</td>
      <td>666773</td>
      <td>217581231</td>
    </tr>
    <tr>
      <th>231</th>
      <td>Into the Wild</td>
      <td>2007</td>
      <td>R</td>
      <td>148</td>
      <td>Adventure, Biography, Drama</td>
      <td>8.1</td>
      <td>After graduating from Emory University, top st...</td>
      <td>73.00000</td>
      <td>Sean Penn</td>
      <td>Emile Hirsch</td>
      <td>Vince Vaughn</td>
      <td>Catherine Keener</td>
      <td>Marcia Gay Harden</td>
      <td>572921</td>
      <td>18354356</td>
    </tr>
    <tr>
      <th>232</th>
      <td>No Country for Old Men</td>
      <td>2007</td>
      <td>R</td>
      <td>122</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.1</td>
      <td>Violence and mayhem ensue after a hunter stumb...</td>
      <td>91.00000</td>
      <td>Ethan Coen</td>
      <td>Joel Coen</td>
      <td>Tommy Lee Jones</td>
      <td>Javier Bardem</td>
      <td>Josh Brolin</td>
      <td>856916</td>
      <td>74283625</td>
    </tr>
    <tr>
      <th>233</th>
      <td>Lage Raho Munna Bhai</td>
      <td>2006</td>
      <td>U</td>
      <td>144</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.1</td>
      <td>Munna Bhai embarks on a journey with Mahatma G...</td>
      <td>77.97153</td>
      <td>Rajkumar Hirani</td>
      <td>Sanjay Dutt</td>
      <td>Arshad Warsi</td>
      <td>Vidya Balan</td>
      <td>Boman Irani</td>
      <td>43137</td>
      <td>2217561</td>
    </tr>
    <tr>
      <th>234</th>
      <td>Million Dollar Baby</td>
      <td>2004</td>
      <td>UA</td>
      <td>132</td>
      <td>Drama, Sport</td>
      <td>8.1</td>
      <td>A determined woman works with a hardened boxin...</td>
      <td>86.00000</td>
      <td>Clint Eastwood</td>
      <td>Hilary Swank</td>
      <td>Clint Eastwood</td>
      <td>Morgan Freeman</td>
      <td>Jay Baruchel</td>
      <td>635975</td>
      <td>100492203</td>
    </tr>
    <tr>
      <th>235</th>
      <td>Hotel Rwanda</td>
      <td>2004</td>
      <td>PG-13</td>
      <td>121</td>
      <td>Biography, Drama, History</td>
      <td>8.1</td>
      <td>Paul Rusesabagina, a hotel manager, houses ove...</td>
      <td>79.00000</td>
      <td>Terry George</td>
      <td>Don Cheadle</td>
      <td>Sophie Okonedo</td>
      <td>Joaquin Phoenix</td>
      <td>Xolani Mali</td>
      <td>334320</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>236</th>
      <td>Taegukgi hwinalrimyeo</td>
      <td>2004</td>
      <td>R</td>
      <td>140</td>
      <td>Action, Drama, War</td>
      <td>8.1</td>
      <td>When two brothers are forced to fight in the K...</td>
      <td>64.00000</td>
      <td>Je-kyu Kang</td>
      <td>Jang Dong-Gun</td>
      <td>Won Bin</td>
      <td>Eun-ju Lee</td>
      <td>Hyeong-jin Kong</td>
      <td>37820</td>
      <td>1111061</td>
    </tr>
    <tr>
      <th>237</th>
      <td>Before Sunset</td>
      <td>2004</td>
      <td>R</td>
      <td>80</td>
      <td>Drama, Romance</td>
      <td>8.1</td>
      <td>Nine years after Jesse and Celine first met, t...</td>
      <td>90.00000</td>
      <td>Richard Linklater</td>
      <td>Ethan Hawke</td>
      <td>Julie Delpy</td>
      <td>Vernon Dobtcheff</td>
      <td>Louise Lemoine Torrès</td>
      <td>236311</td>
      <td>5820649</td>
    </tr>
    <tr>
      <th>238</th>
      <td>Munna Bhai M.B.B.S.</td>
      <td>2003</td>
      <td>U</td>
      <td>156</td>
      <td>Comedy, Drama, Musical</td>
      <td>8.1</td>
      <td>A gangster sets out to fulfill his father's dr...</td>
      <td>77.97153</td>
      <td>Rajkumar Hirani</td>
      <td>Sanjay Dutt</td>
      <td>Arshad Warsi</td>
      <td>Gracy Singh</td>
      <td>Sunil Dutt</td>
      <td>73992</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>239</th>
      <td>Salinui chueok</td>
      <td>2003</td>
      <td>UA</td>
      <td>131</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.1</td>
      <td>In a small Korean province in 1986, two detect...</td>
      <td>82.00000</td>
      <td>Bong Joon Ho</td>
      <td>Kang-ho Song</td>
      <td>Kim Sang-kyung</td>
      <td>Roe-ha Kim</td>
      <td>Jae-ho Song</td>
      <td>139558</td>
      <td>14131</td>
    </tr>
    <tr>
      <th>240</th>
      <td>Dil Chahta Hai</td>
      <td>2001</td>
      <td>Unrated</td>
      <td>183</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.1</td>
      <td>Three inseparable childhood friends are just o...</td>
      <td>77.97153</td>
      <td>Farhan Akhtar</td>
      <td>Aamir Khan</td>
      <td>Saif Ali Khan</td>
      <td>Akshaye Khanna</td>
      <td>Preity Zinta</td>
      <td>66803</td>
      <td>300000</td>
    </tr>
    <tr>
      <th>241</th>
      <td>Kill Bill: Vol. 1</td>
      <td>2003</td>
      <td>R</td>
      <td>111</td>
      <td>Action, Crime, Drama</td>
      <td>8.1</td>
      <td>After awakening from a four-year coma, a forme...</td>
      <td>69.00000</td>
      <td>Quentin Tarantino</td>
      <td>Uma Thurman</td>
      <td>David Carradine</td>
      <td>Daryl Hannah</td>
      <td>Michael Madsen</td>
      <td>1000639</td>
      <td>70099045</td>
    </tr>
    <tr>
      <th>242</th>
      <td>Finding Nemo</td>
      <td>2003</td>
      <td>U</td>
      <td>100</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.1</td>
      <td>After his son is captured in the Great Barrier...</td>
      <td>90.00000</td>
      <td>Andrew Stanton</td>
      <td>Lee Unkrich</td>
      <td>Albert Brooks</td>
      <td>Ellen DeGeneres</td>
      <td>Alexander Gould</td>
      <td>949565</td>
      <td>380843261</td>
    </tr>
    <tr>
      <th>243</th>
      <td>Catch Me If You Can</td>
      <td>2002</td>
      <td>A</td>
      <td>141</td>
      <td>Biography, Crime, Drama</td>
      <td>8.1</td>
      <td>Barely 21 yet, Frank is a skilled forger who h...</td>
      <td>75.00000</td>
      <td>Steven Spielberg</td>
      <td>Leonardo DiCaprio</td>
      <td>Tom Hanks</td>
      <td>Christopher Walken</td>
      <td>Martin Sheen</td>
      <td>832846</td>
      <td>164615351</td>
    </tr>
    <tr>
      <th>244</th>
      <td>Amores perros</td>
      <td>2000</td>
      <td>A</td>
      <td>154</td>
      <td>Drama, Thriller</td>
      <td>8.1</td>
      <td>A horrific car accident connects three stories...</td>
      <td>83.00000</td>
      <td>Alejandro G. Iñárritu</td>
      <td>Emilio Echevarría</td>
      <td>Gael García Bernal</td>
      <td>Goya Toledo</td>
      <td>Álvaro Guerrero</td>
      <td>223741</td>
      <td>5383834</td>
    </tr>
    <tr>
      <th>245</th>
      <td>Monsters, Inc.</td>
      <td>2001</td>
      <td>U</td>
      <td>92</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.1</td>
      <td>In order to power the city, monsters have to s...</td>
      <td>79.00000</td>
      <td>Pete Docter</td>
      <td>David Silverman</td>
      <td>Lee Unkrich</td>
      <td>Billy Crystal</td>
      <td>John Goodman</td>
      <td>815505</td>
      <td>289916256</td>
    </tr>
    <tr>
      <th>246</th>
      <td>Shin seiki Evangelion Gekijô-ban: Air/Magokoro...</td>
      <td>1997</td>
      <td>UA</td>
      <td>87</td>
      <td>Animation, Action, Drama</td>
      <td>8.1</td>
      <td>Concurrent theatrical ending of the TV series ...</td>
      <td>77.97153</td>
      <td>Hideaki Anno</td>
      <td>Kazuya Tsurumaki</td>
      <td>Megumi Ogata</td>
      <td>Megumi Hayashibara</td>
      <td>Yûko Miyamura</td>
      <td>38847</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>247</th>
      <td>Lagaan: Once Upon a Time in India</td>
      <td>2001</td>
      <td>U</td>
      <td>224</td>
      <td>Adventure, Drama, Musical</td>
      <td>8.1</td>
      <td>The people of a small village in Victorian Ind...</td>
      <td>84.00000</td>
      <td>Ashutosh Gowariker</td>
      <td>Aamir Khan</td>
      <td>Raghuvir Yadav</td>
      <td>Gracy Singh</td>
      <td>Rachel Shelley</td>
      <td>105036</td>
      <td>70147</td>
    </tr>
    <tr>
      <th>248</th>
      <td>The Sixth Sense</td>
      <td>1999</td>
      <td>A</td>
      <td>107</td>
      <td>Drama, Mystery, Thriller</td>
      <td>8.1</td>
      <td>A boy who communicates with spirits seeks the ...</td>
      <td>64.00000</td>
      <td>M. Night Shyamalan</td>
      <td>Bruce Willis</td>
      <td>Haley Joel Osment</td>
      <td>Toni Collette</td>
      <td>Olivia Williams</td>
      <td>911573</td>
      <td>293506292</td>
    </tr>
    <tr>
      <th>249</th>
      <td>La leggenda del pianista sull'oceano</td>
      <td>1998</td>
      <td>U</td>
      <td>169</td>
      <td>Drama, Music, Romance</td>
      <td>8.1</td>
      <td>A baby boy, discovered in 1900 on an ocean lin...</td>
      <td>58.00000</td>
      <td>Giuseppe Tornatore</td>
      <td>Tim Roth</td>
      <td>Pruitt Taylor Vince</td>
      <td>Mélanie Thierry</td>
      <td>Bill Nunn</td>
      <td>59020</td>
      <td>259127</td>
    </tr>
    <tr>
      <th>250</th>
      <td>The Truman Show</td>
      <td>1998</td>
      <td>U</td>
      <td>103</td>
      <td>Comedy, Drama</td>
      <td>8.1</td>
      <td>An insurance salesman discovers his whole life...</td>
      <td>90.00000</td>
      <td>Peter Weir</td>
      <td>Jim Carrey</td>
      <td>Ed Harris</td>
      <td>Laura Linney</td>
      <td>Noah Emmerich</td>
      <td>939631</td>
      <td>125618201</td>
    </tr>
    <tr>
      <th>251</th>
      <td>Crna macka, beli macor</td>
      <td>1998</td>
      <td>R</td>
      <td>127</td>
      <td>Comedy, Crime, Romance</td>
      <td>8.1</td>
      <td>Matko and his son Zare live on the banks of th...</td>
      <td>73.00000</td>
      <td>Emir Kusturica</td>
      <td>Bajram Severdzan</td>
      <td>Srdjan 'Zika' Todorovic</td>
      <td>Branka Katic</td>
      <td>Florijan Ajdini</td>
      <td>50862</td>
      <td>348660</td>
    </tr>
    <tr>
      <th>252</th>
      <td>The Big Lebowski</td>
      <td>1998</td>
      <td>R</td>
      <td>117</td>
      <td>Comedy, Crime, Sport</td>
      <td>8.1</td>
      <td>Jeff "The Dude" Lebowski, mistaken for a milli...</td>
      <td>71.00000</td>
      <td>Joel Coen</td>
      <td>Ethan Coen</td>
      <td>Jeff Bridges</td>
      <td>John Goodman</td>
      <td>Julianne Moore</td>
      <td>732620</td>
      <td>17498804</td>
    </tr>
    <tr>
      <th>253</th>
      <td>Fa yeung nin wah</td>
      <td>2000</td>
      <td>U</td>
      <td>98</td>
      <td>Drama, Romance</td>
      <td>8.1</td>
      <td>Two neighbors, a woman and a man, form a stron...</td>
      <td>85.00000</td>
      <td>Kar-Wai Wong</td>
      <td>Tony Chiu-Wai Leung</td>
      <td>Maggie Cheung</td>
      <td>Ping Lam Siu</td>
      <td>Tung Cho 'Joe' Cheung</td>
      <td>124383</td>
      <td>2734044</td>
    </tr>
    <tr>
      <th>254</th>
      <td>Trainspotting</td>
      <td>1996</td>
      <td>A</td>
      <td>93</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>Renton, deeply immersed in the Edinburgh drug ...</td>
      <td>83.00000</td>
      <td>Danny Boyle</td>
      <td>Ewan McGregor</td>
      <td>Ewen Bremner</td>
      <td>Jonny Lee Miller</td>
      <td>Kevin McKidd</td>
      <td>634716</td>
      <td>16501785</td>
    </tr>
    <tr>
      <th>255</th>
      <td>Fargo</td>
      <td>1996</td>
      <td>A</td>
      <td>98</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.1</td>
      <td>Jerry Lundegaard's inept crime falls apart due...</td>
      <td>85.00000</td>
      <td>Joel Coen</td>
      <td>Ethan Coen</td>
      <td>William H. Macy</td>
      <td>Frances McDormand</td>
      <td>Steve Buscemi</td>
      <td>617444</td>
      <td>24611975</td>
    </tr>
    <tr>
      <th>256</th>
      <td>Underground</td>
      <td>1995</td>
      <td>Unknown</td>
      <td>170</td>
      <td>Comedy, Drama, War</td>
      <td>8.1</td>
      <td>A group of Serbian socialists prepares for the...</td>
      <td>77.97153</td>
      <td>Emir Kusturica</td>
      <td>Predrag 'Miki' Manojlovic</td>
      <td>Lazar Ristovski</td>
      <td>Mirjana Jokovic</td>
      <td>Slavko Stimac</td>
      <td>55220</td>
      <td>171082</td>
    </tr>
    <tr>
      <th>257</th>
      <td>La haine</td>
      <td>1995</td>
      <td>UA</td>
      <td>98</td>
      <td>Crime, Drama</td>
      <td>8.1</td>
      <td>24 hours in the lives of three young men in th...</td>
      <td>77.97153</td>
      <td>Mathieu Kassovitz</td>
      <td>Vincent Cassel</td>
      <td>Hubert Koundé</td>
      <td>Saïd Taghmaoui</td>
      <td>Abdel Ahmed Ghili</td>
      <td>150345</td>
      <td>309811</td>
    </tr>
    <tr>
      <th>258</th>
      <td>Dilwale Dulhania Le Jayenge</td>
      <td>1995</td>
      <td>U</td>
      <td>189</td>
      <td>Drama, Romance</td>
      <td>8.1</td>
      <td>When Raj meets Simran in Europe, it isn't love...</td>
      <td>77.97153</td>
      <td>Aditya Chopra</td>
      <td>Shah Rukh Khan</td>
      <td>Kajol</td>
      <td>Amrish Puri</td>
      <td>Farida Jalal</td>
      <td>63516</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>259</th>
      <td>Before Sunrise</td>
      <td>1995</td>
      <td>R</td>
      <td>101</td>
      <td>Drama, Romance</td>
      <td>8.1</td>
      <td>A young man and woman meet on a train in Europ...</td>
      <td>77.00000</td>
      <td>Richard Linklater</td>
      <td>Ethan Hawke</td>
      <td>Julie Delpy</td>
      <td>Andrea Eckert</td>
      <td>Hanno Pöschl</td>
      <td>272291</td>
      <td>5535405</td>
    </tr>
    <tr>
      <th>260</th>
      <td>Trois couleurs: Rouge</td>
      <td>1994</td>
      <td>U</td>
      <td>99</td>
      <td>Drama, Mystery, Romance</td>
      <td>8.1</td>
      <td>A model discovers a retired judge is keen on i...</td>
      <td>100.00000</td>
      <td>Krzysztof Kieslowski</td>
      <td>Irène Jacob</td>
      <td>Jean-Louis Trintignant</td>
      <td>Frédérique Feder</td>
      <td>Jean-Pierre Lorit</td>
      <td>90729</td>
      <td>4043686</td>
    </tr>
    <tr>
      <th>261</th>
      <td>Chung Hing sam lam</td>
      <td>1994</td>
      <td>U</td>
      <td>102</td>
      <td>Comedy, Crime, Drama</td>
      <td>8.1</td>
      <td>Two melancholy Hong Kong policemen fall in lov...</td>
      <td>77.00000</td>
      <td>Kar-Wai Wong</td>
      <td>Brigitte Lin</td>
      <td>Takeshi Kaneshiro</td>
      <td>Tony Chiu-Wai Leung</td>
      <td>Faye Wong</td>
      <td>63122</td>
      <td>600200</td>
    </tr>
    <tr>
      <th>262</th>
      <td>Jurassic Park</td>
      <td>1993</td>
      <td>UA</td>
      <td>127</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>8.1</td>
      <td>A pragmatic paleontologist visiting an almost ...</td>
      <td>68.00000</td>
      <td>Steven Spielberg</td>
      <td>Sam Neill</td>
      <td>Laura Dern</td>
      <td>Jeff Goldblum</td>
      <td>Richard Attenborough</td>
      <td>867615</td>
      <td>402453882</td>
    </tr>
    <tr>
      <th>263</th>
      <td>In the Name of the Father</td>
      <td>1993</td>
      <td>UA</td>
      <td>133</td>
      <td>Biography, Crime, Drama</td>
      <td>8.1</td>
      <td>A man's coerced confession to an I.R.A. bombin...</td>
      <td>84.00000</td>
      <td>Jim Sheridan</td>
      <td>Daniel Day-Lewis</td>
      <td>Pete Postlethwaite</td>
      <td>Alison Crosbie</td>
      <td>Philip King</td>
      <td>156842</td>
      <td>25010410</td>
    </tr>
    <tr>
      <th>264</th>
      <td>Ba wang bie ji</td>
      <td>1993</td>
      <td>R</td>
      <td>171</td>
      <td>Drama, Music, Romance</td>
      <td>8.1</td>
      <td>Two boys meet at an opera training school in P...</td>
      <td>77.97153</td>
      <td>Kaige Chen</td>
      <td>Leslie Cheung</td>
      <td>Fengyi Zhang</td>
      <td>Gong Li</td>
      <td>You Ge</td>
      <td>25088</td>
      <td>5216888</td>
    </tr>
    <tr>
      <th>265</th>
      <td>Dà hóng denglong gaogao guà</td>
      <td>1991</td>
      <td>PG</td>
      <td>125</td>
      <td>Drama, History, Romance</td>
      <td>8.1</td>
      <td>A young woman becomes the fourth wife of a wea...</td>
      <td>77.97153</td>
      <td>Yimou Zhang</td>
      <td>Gong Li</td>
      <td>Jingwu Ma</td>
      <td>Saifei He</td>
      <td>Cuifen Cao</td>
      <td>29662</td>
      <td>2603061</td>
    </tr>
    <tr>
      <th>266</th>
      <td>Dead Poets Society</td>
      <td>1989</td>
      <td>U</td>
      <td>128</td>
      <td>Comedy, Drama</td>
      <td>8.1</td>
      <td>Maverick teacher John Keating uses poetry to e...</td>
      <td>79.00000</td>
      <td>Peter Weir</td>
      <td>Robin Williams</td>
      <td>Robert Sean Leonard</td>
      <td>Ethan Hawke</td>
      <td>Josh Charles</td>
      <td>425457</td>
      <td>95860116</td>
    </tr>
    <tr>
      <th>267</th>
      <td>Stand by Me</td>
      <td>1986</td>
      <td>U</td>
      <td>89</td>
      <td>Adventure, Drama</td>
      <td>8.1</td>
      <td>After the death of one of his friends, a write...</td>
      <td>75.00000</td>
      <td>Rob Reiner</td>
      <td>Wil Wheaton</td>
      <td>River Phoenix</td>
      <td>Corey Feldman</td>
      <td>Jerry O'Connell</td>
      <td>363401</td>
      <td>52287414</td>
    </tr>
    <tr>
      <th>268</th>
      <td>Platoon</td>
      <td>1986</td>
      <td>A</td>
      <td>120</td>
      <td>Drama, War</td>
      <td>8.1</td>
      <td>Chris Taylor, a neophyte recruit in Vietnam, f...</td>
      <td>92.00000</td>
      <td>Oliver Stone</td>
      <td>Charlie Sheen</td>
      <td>Tom Berenger</td>
      <td>Willem Dafoe</td>
      <td>Keith David</td>
      <td>381222</td>
      <td>138530565</td>
    </tr>
    <tr>
      <th>269</th>
      <td>Paris, Texas</td>
      <td>1984</td>
      <td>U</td>
      <td>145</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>Travis Henderson, an aimless drifter who has b...</td>
      <td>78.00000</td>
      <td>Wim Wenders</td>
      <td>Harry Dean Stanton</td>
      <td>Nastassja Kinski</td>
      <td>Dean Stockwell</td>
      <td>Aurore Clément</td>
      <td>91188</td>
      <td>2181987</td>
    </tr>
    <tr>
      <th>270</th>
      <td>Kaze no tani no Naushika</td>
      <td>1984</td>
      <td>U</td>
      <td>117</td>
      <td>Animation, Adventure, Fantasy</td>
      <td>8.1</td>
      <td>Warrior and pacifist Princess Nausicaä despera...</td>
      <td>86.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Sumi Shimamoto</td>
      <td>Mahito Tsujimura</td>
      <td>Hisako Kyôda</td>
      <td>Gorô Naya</td>
      <td>150924</td>
      <td>495770</td>
    </tr>
    <tr>
      <th>271</th>
      <td>The Thing</td>
      <td>1982</td>
      <td>A</td>
      <td>109</td>
      <td>Horror, Mystery, Sci-Fi</td>
      <td>8.1</td>
      <td>A research team in Antarctica is hunted by a s...</td>
      <td>57.00000</td>
      <td>John Carpenter</td>
      <td>Kurt Russell</td>
      <td>Wilford Brimley</td>
      <td>Keith David</td>
      <td>Richard Masur</td>
      <td>371271</td>
      <td>13782838</td>
    </tr>
    <tr>
      <th>272</th>
      <td>Pink Floyd: The Wall</td>
      <td>1982</td>
      <td>UA</td>
      <td>95</td>
      <td>Drama, Fantasy, Music</td>
      <td>8.1</td>
      <td>A confined but troubled rock star descends int...</td>
      <td>47.00000</td>
      <td>Alan Parker</td>
      <td>Bob Geldof</td>
      <td>Christine Hargreaves</td>
      <td>James Laurenson</td>
      <td>Eleanor David</td>
      <td>76081</td>
      <td>22244207</td>
    </tr>
    <tr>
      <th>273</th>
      <td>Fitzcarraldo</td>
      <td>1982</td>
      <td>R</td>
      <td>158</td>
      <td>Adventure, Drama</td>
      <td>8.1</td>
      <td>The story of Brian Sweeney Fitzgerald, an extr...</td>
      <td>77.97153</td>
      <td>Werner Herzog</td>
      <td>Klaus Kinski</td>
      <td>Claudia Cardinale</td>
      <td>José Lewgoy</td>
      <td>Miguel Ángel Fuentes</td>
      <td>31595</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>274</th>
      <td>Fanny och Alexander</td>
      <td>1982</td>
      <td>A</td>
      <td>188</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>Two young Swedish children experience the many...</td>
      <td>100.00000</td>
      <td>Ingmar Bergman</td>
      <td>Bertil Guve</td>
      <td>Pernilla Allwin</td>
      <td>Kristina Adolphson</td>
      <td>Börje Ahlstedt</td>
      <td>57784</td>
      <td>4971340</td>
    </tr>
    <tr>
      <th>275</th>
      <td>Blade Runner</td>
      <td>1982</td>
      <td>UA</td>
      <td>117</td>
      <td>Action, Sci-Fi, Thriller</td>
      <td>8.1</td>
      <td>A blade runner must pursue and terminate four ...</td>
      <td>84.00000</td>
      <td>Ridley Scott</td>
      <td>Harrison Ford</td>
      <td>Rutger Hauer</td>
      <td>Sean Young</td>
      <td>Edward James Olmos</td>
      <td>693827</td>
      <td>32868943</td>
    </tr>
    <tr>
      <th>276</th>
      <td>The Elephant Man</td>
      <td>1980</td>
      <td>UA</td>
      <td>124</td>
      <td>Biography, Drama</td>
      <td>8.1</td>
      <td>A Victorian surgeon rescues a heavily disfigur...</td>
      <td>78.00000</td>
      <td>David Lynch</td>
      <td>Anthony Hopkins</td>
      <td>John Hurt</td>
      <td>Anne Bancroft</td>
      <td>John Gielgud</td>
      <td>220078</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>277</th>
      <td>Life of Brian</td>
      <td>1979</td>
      <td>R</td>
      <td>94</td>
      <td>Comedy</td>
      <td>8.1</td>
      <td>Born on the original Christmas in the stable n...</td>
      <td>77.00000</td>
      <td>Terry Jones</td>
      <td>Graham Chapman</td>
      <td>John Cleese</td>
      <td>Michael Palin</td>
      <td>Terry Gilliam</td>
      <td>367250</td>
      <td>20045115</td>
    </tr>
    <tr>
      <th>278</th>
      <td>The Deer Hunter</td>
      <td>1978</td>
      <td>A</td>
      <td>183</td>
      <td>Drama, War</td>
      <td>8.1</td>
      <td>An in-depth examination of the ways in which t...</td>
      <td>86.00000</td>
      <td>Michael Cimino</td>
      <td>Robert De Niro</td>
      <td>Christopher Walken</td>
      <td>John Cazale</td>
      <td>John Savage</td>
      <td>311361</td>
      <td>48979328</td>
    </tr>
    <tr>
      <th>279</th>
      <td>Rocky</td>
      <td>1976</td>
      <td>U</td>
      <td>120</td>
      <td>Drama, Sport</td>
      <td>8.1</td>
      <td>A small-time boxer gets a supremely rare chanc...</td>
      <td>70.00000</td>
      <td>John G. Avildsen</td>
      <td>Sylvester Stallone</td>
      <td>Talia Shire</td>
      <td>Burt Young</td>
      <td>Carl Weathers</td>
      <td>518546</td>
      <td>117235247</td>
    </tr>
    <tr>
      <th>280</th>
      <td>Network</td>
      <td>1976</td>
      <td>UA</td>
      <td>121</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>A television network cynically exploits a dera...</td>
      <td>83.00000</td>
      <td>Sidney Lumet</td>
      <td>Faye Dunaway</td>
      <td>William Holden</td>
      <td>Peter Finch</td>
      <td>Robert Duvall</td>
      <td>144911</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>281</th>
      <td>Barry Lyndon</td>
      <td>1975</td>
      <td>PG</td>
      <td>185</td>
      <td>Adventure, Drama, History</td>
      <td>8.1</td>
      <td>An Irish rogue wins the heart of a rich widow ...</td>
      <td>89.00000</td>
      <td>Stanley Kubrick</td>
      <td>Ryan O'Neal</td>
      <td>Marisa Berenson</td>
      <td>Patrick Magee</td>
      <td>Hardy Krüger</td>
      <td>149843</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>282</th>
      <td>Zerkalo</td>
      <td>1975</td>
      <td>G</td>
      <td>107</td>
      <td>Biography, Drama</td>
      <td>8.1</td>
      <td>A dying man in his forties remembers his past....</td>
      <td>77.97153</td>
      <td>Andrei Tarkovsky</td>
      <td>Margarita Terekhova</td>
      <td>Filipp Yankovskiy</td>
      <td>Ignat Daniltsev</td>
      <td>Oleg Yankovskiy</td>
      <td>40081</td>
      <td>177345</td>
    </tr>
    <tr>
      <th>283</th>
      <td>Chinatown</td>
      <td>1974</td>
      <td>UA</td>
      <td>130</td>
      <td>Drama, Mystery, Thriller</td>
      <td>8.1</td>
      <td>A private detective hired to expose an adulter...</td>
      <td>92.00000</td>
      <td>Roman Polanski</td>
      <td>Jack Nicholson</td>
      <td>Faye Dunaway</td>
      <td>John Huston</td>
      <td>Perry Lopez</td>
      <td>294230</td>
      <td>29000000</td>
    </tr>
    <tr>
      <th>284</th>
      <td>Paper Moon</td>
      <td>1973</td>
      <td>U</td>
      <td>102</td>
      <td>Comedy, Crime, Drama</td>
      <td>8.1</td>
      <td>During the Great Depression, a con man finds h...</td>
      <td>77.00000</td>
      <td>Peter Bogdanovich</td>
      <td>Ryan O'Neal</td>
      <td>Tatum O'Neal</td>
      <td>Madeline Kahn</td>
      <td>John Hillerman</td>
      <td>42285</td>
      <td>30933743</td>
    </tr>
    <tr>
      <th>285</th>
      <td>Viskningar och rop</td>
      <td>1972</td>
      <td>A</td>
      <td>91</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>When a woman dying of cancer in early twentiet...</td>
      <td>77.97153</td>
      <td>Ingmar Bergman</td>
      <td>Harriet Andersson</td>
      <td>Liv Ullmann</td>
      <td>Kari Sylwan</td>
      <td>Ingrid Thulin</td>
      <td>30206</td>
      <td>1742348</td>
    </tr>
    <tr>
      <th>286</th>
      <td>Solaris</td>
      <td>1972</td>
      <td>PG</td>
      <td>167</td>
      <td>Drama, Mystery, Sci-Fi</td>
      <td>8.1</td>
      <td>A psychologist is sent to a station orbiting a...</td>
      <td>90.00000</td>
      <td>Andrei Tarkovsky</td>
      <td>Natalya Bondarchuk</td>
      <td>Donatas Banionis</td>
      <td>Jüri Järvet</td>
      <td>Vladislav Dvorzhetskiy</td>
      <td>81021</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>287</th>
      <td>Le samouraï</td>
      <td>1967</td>
      <td>GP</td>
      <td>105</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.1</td>
      <td>After professional hitman Jef Costello is seen...</td>
      <td>77.97153</td>
      <td>Jean-Pierre Melville</td>
      <td>Alain Delon</td>
      <td>François Périer</td>
      <td>Nathalie Delon</td>
      <td>Cathy Rosier</td>
      <td>45434</td>
      <td>39481</td>
    </tr>
    <tr>
      <th>288</th>
      <td>Cool Hand Luke</td>
      <td>1967</td>
      <td>A</td>
      <td>127</td>
      <td>Crime, Drama</td>
      <td>8.1</td>
      <td>A laid back Southern man is sentenced to two y...</td>
      <td>92.00000</td>
      <td>Stuart Rosenberg</td>
      <td>Paul Newman</td>
      <td>George Kennedy</td>
      <td>Strother Martin</td>
      <td>J.D. Cannon</td>
      <td>161984</td>
      <td>16217773</td>
    </tr>
    <tr>
      <th>289</th>
      <td>Persona</td>
      <td>1966</td>
      <td>Unknown</td>
      <td>85</td>
      <td>Drama, Thriller</td>
      <td>8.1</td>
      <td>A nurse is put in charge of a mute actress and...</td>
      <td>86.00000</td>
      <td>Ingmar Bergman</td>
      <td>Bibi Andersson</td>
      <td>Liv Ullmann</td>
      <td>Margaretha Krook</td>
      <td>Gunnar Björnstrand</td>
      <td>103191</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>290</th>
      <td>Andrei Rublev</td>
      <td>1966</td>
      <td>R</td>
      <td>205</td>
      <td>Biography, Drama, History</td>
      <td>8.1</td>
      <td>The life, times and afflictions of the fifteen...</td>
      <td>77.97153</td>
      <td>Andrei Tarkovsky</td>
      <td>Anatoliy Solonitsyn</td>
      <td>Ivan Lapikov</td>
      <td>Nikolay Grinko</td>
      <td>Nikolay Sergeev</td>
      <td>46947</td>
      <td>102021</td>
    </tr>
    <tr>
      <th>291</th>
      <td>La battaglia di Algeri</td>
      <td>1966</td>
      <td>Unknown</td>
      <td>121</td>
      <td>Drama, War</td>
      <td>8.1</td>
      <td>In the 1950s, fear and violence escalate as th...</td>
      <td>96.00000</td>
      <td>Gillo Pontecorvo</td>
      <td>Brahim Hadjadj</td>
      <td>Jean Martin</td>
      <td>Yacef Saadi</td>
      <td>Samia Kerbash</td>
      <td>53089</td>
      <td>55908</td>
    </tr>
    <tr>
      <th>292</th>
      <td>El ángel exterminador</td>
      <td>1962</td>
      <td>Unknown</td>
      <td>95</td>
      <td>Drama, Fantasy</td>
      <td>8.1</td>
      <td>The guests at an upper-class dinner party find...</td>
      <td>77.97153</td>
      <td>Luis Buñuel</td>
      <td>Silvia Pinal</td>
      <td>Jacqueline Andere</td>
      <td>Enrique Rambal</td>
      <td>José Baviera</td>
      <td>29682</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>293</th>
      <td>What Ever Happened to Baby Jane?</td>
      <td>1962</td>
      <td>Passed</td>
      <td>134</td>
      <td>Drama, Horror, Thriller</td>
      <td>8.1</td>
      <td>A former child star torments her paraplegic si...</td>
      <td>75.00000</td>
      <td>Robert Aldrich</td>
      <td>Bette Davis</td>
      <td>Joan Crawford</td>
      <td>Victor Buono</td>
      <td>Wesley Addy</td>
      <td>50058</td>
      <td>4050000</td>
    </tr>
    <tr>
      <th>294</th>
      <td>Sanjuro</td>
      <td>1962</td>
      <td>U</td>
      <td>96</td>
      <td>Action, Comedy, Crime</td>
      <td>8.1</td>
      <td>A crafty samurai helps a young man and his fel...</td>
      <td>77.97153</td>
      <td>Akira Kurosawa</td>
      <td>Toshirô Mifune</td>
      <td>Tatsuya Nakadai</td>
      <td>Keiju Kobayashi</td>
      <td>Yûnosuke Itô</td>
      <td>33044</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>295</th>
      <td>The Man Who Shot Liberty Valance</td>
      <td>1962</td>
      <td>Unknown</td>
      <td>123</td>
      <td>Drama, Western</td>
      <td>8.1</td>
      <td>A senator returns to a western town for the fu...</td>
      <td>94.00000</td>
      <td>John Ford</td>
      <td>James Stewart</td>
      <td>John Wayne</td>
      <td>Vera Miles</td>
      <td>Lee Marvin</td>
      <td>68827</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>296</th>
      <td>Ivanovo detstvo</td>
      <td>1962</td>
      <td>Unknown</td>
      <td>95</td>
      <td>Drama, War</td>
      <td>8.1</td>
      <td>In WW2, twelve year old Soviet orphan Ivan Bon...</td>
      <td>77.97153</td>
      <td>Andrei Tarkovsky</td>
      <td>Eduard Abalov</td>
      <td>Nikolay Burlyaev</td>
      <td>Valentin Zubkov</td>
      <td>Evgeniy Zharikov</td>
      <td>31728</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>297</th>
      <td>Jungfrukällan</td>
      <td>1960</td>
      <td>A</td>
      <td>89</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>An innocent yet pampered young virgin and her ...</td>
      <td>77.97153</td>
      <td>Ingmar Bergman</td>
      <td>Max von Sydow</td>
      <td>Birgitta Valberg</td>
      <td>Gunnel Lindblom</td>
      <td>Birgitta Pettersson</td>
      <td>26697</td>
      <td>1526000</td>
    </tr>
    <tr>
      <th>298</th>
      <td>Inherit the Wind</td>
      <td>1960</td>
      <td>Passed</td>
      <td>128</td>
      <td>Biography, Drama, History</td>
      <td>8.1</td>
      <td>Based on a real-life case in 1925, two great l...</td>
      <td>75.00000</td>
      <td>Stanley Kramer</td>
      <td>Spencer Tracy</td>
      <td>Fredric March</td>
      <td>Gene Kelly</td>
      <td>Dick York</td>
      <td>27254</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>299</th>
      <td>Les quatre cents coups</td>
      <td>1959</td>
      <td>Unknown</td>
      <td>99</td>
      <td>Crime, Drama</td>
      <td>8.1</td>
      <td>A young boy, left without attention, delves in...</td>
      <td>77.97153</td>
      <td>François Truffaut</td>
      <td>Jean-Pierre Léaud</td>
      <td>Albert Rémy</td>
      <td>Claire Maurier</td>
      <td>Guy Decomble</td>
      <td>105291</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>300</th>
      <td>Ben-Hur</td>
      <td>1959</td>
      <td>U</td>
      <td>212</td>
      <td>Adventure, Drama, History</td>
      <td>8.1</td>
      <td>After a Jewish prince is betrayed and sent int...</td>
      <td>90.00000</td>
      <td>William Wyler</td>
      <td>Charlton Heston</td>
      <td>Jack Hawkins</td>
      <td>Stephen Boyd</td>
      <td>Haya Harareet</td>
      <td>219466</td>
      <td>74700000</td>
    </tr>
    <tr>
      <th>301</th>
      <td>Kakushi-toride no san-akunin</td>
      <td>1958</td>
      <td>Unknown</td>
      <td>139</td>
      <td>Adventure, Drama</td>
      <td>8.1</td>
      <td>Lured by gold, two greedy peasants unknowingly...</td>
      <td>77.97153</td>
      <td>Akira Kurosawa</td>
      <td>Toshirô Mifune</td>
      <td>Misa Uehara</td>
      <td>Minoru Chiaki</td>
      <td>Kamatari Fujiwara</td>
      <td>34797</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>302</th>
      <td>Le notti di Cabiria</td>
      <td>1957</td>
      <td>Unknown</td>
      <td>110</td>
      <td>Drama</td>
      <td>8.1</td>
      <td>A waifish prostitute wanders the streets of Ro...</td>
      <td>77.97153</td>
      <td>Federico Fellini</td>
      <td>Giulietta Masina</td>
      <td>François Périer</td>
      <td>Franca Marzi</td>
      <td>Dorian Gray</td>
      <td>42940</td>
      <td>752045</td>
    </tr>
    <tr>
      <th>303</th>
      <td>Kumonosu-jô</td>
      <td>1957</td>
      <td>Unknown</td>
      <td>110</td>
      <td>Drama, History</td>
      <td>8.1</td>
      <td>A war-hardened general, egged on by his ambiti...</td>
      <td>77.97153</td>
      <td>Akira Kurosawa</td>
      <td>Toshirô Mifune</td>
      <td>Minoru Chiaki</td>
      <td>Isuzu Yamada</td>
      <td>Takashi Shimura</td>
      <td>46678</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>304</th>
      <td>The Bridge on the River Kwai</td>
      <td>1957</td>
      <td>PG</td>
      <td>161</td>
      <td>Adventure, Drama, War</td>
      <td>8.1</td>
      <td>British POWs are forced to build a railway bri...</td>
      <td>87.00000</td>
      <td>David Lean</td>
      <td>William Holden</td>
      <td>Alec Guinness</td>
      <td>Jack Hawkins</td>
      <td>Sessue Hayakawa</td>
      <td>203463</td>
      <td>44908000</td>
    </tr>
    <tr>
      <th>305</th>
      <td>On the Waterfront</td>
      <td>1954</td>
      <td>A</td>
      <td>108</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.1</td>
      <td>An ex-prize fighter turned longshoreman strugg...</td>
      <td>91.00000</td>
      <td>Elia Kazan</td>
      <td>Marlon Brando</td>
      <td>Karl Malden</td>
      <td>Lee J. Cobb</td>
      <td>Rod Steiger</td>
      <td>142107</td>
      <td>9600000</td>
    </tr>
    <tr>
      <th>306</th>
      <td>Le salaire de la peur</td>
      <td>1953</td>
      <td>U</td>
      <td>131</td>
      <td>Adventure, Drama, Thriller</td>
      <td>8.1</td>
      <td>In a decrepit South American village, four men...</td>
      <td>85.00000</td>
      <td>Henri-Georges Clouzot</td>
      <td>Yves Montand</td>
      <td>Charles Vanel</td>
      <td>Peter van Eyck</td>
      <td>Folco Lulli</td>
      <td>54588</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>307</th>
      <td>Ace in the Hole</td>
      <td>1951</td>
      <td>Approved</td>
      <td>111</td>
      <td>Drama, Film-Noir</td>
      <td>8.1</td>
      <td>A frustrated former big-city journalist now st...</td>
      <td>72.00000</td>
      <td>Billy Wilder</td>
      <td>Kirk Douglas</td>
      <td>Jan Sterling</td>
      <td>Robert Arthur</td>
      <td>Porter Hall</td>
      <td>31568</td>
      <td>3969893</td>
    </tr>
    <tr>
      <th>308</th>
      <td>White Heat</td>
      <td>1949</td>
      <td>Unknown</td>
      <td>114</td>
      <td>Action, Crime, Drama</td>
      <td>8.1</td>
      <td>A psychopathic criminal with a mother complex ...</td>
      <td>77.97153</td>
      <td>Raoul Walsh</td>
      <td>James Cagney</td>
      <td>Virginia Mayo</td>
      <td>Edmond O'Brien</td>
      <td>Margaret Wycherly</td>
      <td>29807</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>309</th>
      <td>The Third Man</td>
      <td>1949</td>
      <td>Approved</td>
      <td>104</td>
      <td>Film-Noir, Mystery, Thriller</td>
      <td>8.1</td>
      <td>Pulp novelist Holly Martins travels to shadowy...</td>
      <td>97.00000</td>
      <td>Carol Reed</td>
      <td>Orson Welles</td>
      <td>Joseph Cotten</td>
      <td>Alida Valli</td>
      <td>Trevor Howard</td>
      <td>158731</td>
      <td>449191</td>
    </tr>
    <tr>
      <th>310</th>
      <td>The Red Shoes</td>
      <td>1948</td>
      <td>Unknown</td>
      <td>135</td>
      <td>Drama, Music, Romance</td>
      <td>8.1</td>
      <td>A young ballet dancer is torn between the man ...</td>
      <td>77.97153</td>
      <td>Michael Powell</td>
      <td>Emeric Pressburger</td>
      <td>Anton Walbrook</td>
      <td>Marius Goring</td>
      <td>Moira Shearer</td>
      <td>30935</td>
      <td>10900000</td>
    </tr>
    <tr>
      <th>311</th>
      <td>The Shop Around the Corner</td>
      <td>1940</td>
      <td>Unknown</td>
      <td>99</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.1</td>
      <td>Two employees at a gift shop can barely stand ...</td>
      <td>96.00000</td>
      <td>Ernst Lubitsch</td>
      <td>Margaret Sullavan</td>
      <td>James Stewart</td>
      <td>Frank Morgan</td>
      <td>Joseph Schildkraut</td>
      <td>28450</td>
      <td>203300</td>
    </tr>
    <tr>
      <th>312</th>
      <td>Rebecca</td>
      <td>1940</td>
      <td>Approved</td>
      <td>130</td>
      <td>Drama, Mystery, Romance</td>
      <td>8.1</td>
      <td>A self-conscious woman juggles adjusting to he...</td>
      <td>86.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Laurence Olivier</td>
      <td>Joan Fontaine</td>
      <td>George Sanders</td>
      <td>Judith Anderson</td>
      <td>123942</td>
      <td>4360000</td>
    </tr>
    <tr>
      <th>313</th>
      <td>Mr. Smith Goes to Washington</td>
      <td>1939</td>
      <td>Passed</td>
      <td>129</td>
      <td>Comedy, Drama</td>
      <td>8.1</td>
      <td>A naive man is appointed to fill a vacancy in ...</td>
      <td>73.00000</td>
      <td>Frank Capra</td>
      <td>James Stewart</td>
      <td>Jean Arthur</td>
      <td>Claude Rains</td>
      <td>Edward Arnold</td>
      <td>107017</td>
      <td>9600000</td>
    </tr>
    <tr>
      <th>314</th>
      <td>Gone with the Wind</td>
      <td>1939</td>
      <td>U</td>
      <td>238</td>
      <td>Drama, History, Romance</td>
      <td>8.1</td>
      <td>A manipulative woman and a roguish man conduct...</td>
      <td>97.00000</td>
      <td>Victor Fleming</td>
      <td>George Cukor</td>
      <td>Sam Wood</td>
      <td>Clark Gable</td>
      <td>Vivien Leigh</td>
      <td>290074</td>
      <td>198676459</td>
    </tr>
    <tr>
      <th>315</th>
      <td>La Grande Illusion</td>
      <td>1937</td>
      <td>Unknown</td>
      <td>113</td>
      <td>Drama, War</td>
      <td>8.1</td>
      <td>During WWI, two French soldiers are captured a...</td>
      <td>77.97153</td>
      <td>Jean Renoir</td>
      <td>Jean Gabin</td>
      <td>Dita Parlo</td>
      <td>Pierre Fresnay</td>
      <td>Erich von Stroheim</td>
      <td>33829</td>
      <td>172885</td>
    </tr>
    <tr>
      <th>316</th>
      <td>It Happened One Night</td>
      <td>1934</td>
      <td>Approved</td>
      <td>105</td>
      <td>Comedy, Romance</td>
      <td>8.1</td>
      <td>A renegade reporter and a crazy young heiress ...</td>
      <td>87.00000</td>
      <td>Frank Capra</td>
      <td>Clark Gable</td>
      <td>Claudette Colbert</td>
      <td>Walter Connolly</td>
      <td>Roscoe Karns</td>
      <td>94016</td>
      <td>4360000</td>
    </tr>
    <tr>
      <th>317</th>
      <td>La passion de Jeanne d'Arc</td>
      <td>1928</td>
      <td>Passed</td>
      <td>110</td>
      <td>Biography, Drama, History</td>
      <td>8.1</td>
      <td>In 1431, Jeanne d'Arc is placed on trial on ch...</td>
      <td>77.97153</td>
      <td>Carl Theodor Dreyer</td>
      <td>Maria Falconetti</td>
      <td>Eugene Silvain</td>
      <td>André Berley</td>
      <td>Maurice Schutz</td>
      <td>47676</td>
      <td>21877</td>
    </tr>
    <tr>
      <th>318</th>
      <td>The Circus</td>
      <td>1928</td>
      <td>Passed</td>
      <td>72</td>
      <td>Comedy, Romance</td>
      <td>8.1</td>
      <td>The Tramp finds work and the girl of his dream...</td>
      <td>90.00000</td>
      <td>Charles Chaplin</td>
      <td>Charles Chaplin</td>
      <td>Merna Kennedy</td>
      <td>Al Ernest Garcia</td>
      <td>Harry Crocker</td>
      <td>30205</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>319</th>
      <td>Sunrise: A Song of Two Humans</td>
      <td>1927</td>
      <td>Passed</td>
      <td>94</td>
      <td>Drama, Romance</td>
      <td>8.1</td>
      <td>An allegorical tale about a man fighting the g...</td>
      <td>77.97153</td>
      <td>F.W. Murnau</td>
      <td>George O'Brien</td>
      <td>Janet Gaynor</td>
      <td>Margaret Livingston</td>
      <td>Bodil Rosing</td>
      <td>46865</td>
      <td>539540</td>
    </tr>
    <tr>
      <th>320</th>
      <td>The General</td>
      <td>1926</td>
      <td>Passed</td>
      <td>67</td>
      <td>Action, Adventure, Comedy</td>
      <td>8.1</td>
      <td>When Union spies steal an engineer's beloved l...</td>
      <td>77.97153</td>
      <td>Clyde Bruckman</td>
      <td>Buster Keaton</td>
      <td>Buster Keaton</td>
      <td>Marion Mack</td>
      <td>Glen Cavender</td>
      <td>81156</td>
      <td>1033895</td>
    </tr>
    <tr>
      <th>321</th>
      <td>Das Cabinet des Dr. Caligari</td>
      <td>1920</td>
      <td>Unknown</td>
      <td>76</td>
      <td>Fantasy, Horror, Mystery</td>
      <td>8.1</td>
      <td>Hypnotist Dr. Caligari uses a somnambulist, Ce...</td>
      <td>77.97153</td>
      <td>Robert Wiene</td>
      <td>Werner Krauss</td>
      <td>Conrad Veidt</td>
      <td>Friedrich Feher</td>
      <td>Lil Dagover</td>
      <td>57428</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>322</th>
      <td>Badhaai ho</td>
      <td>2018</td>
      <td>UA</td>
      <td>124</td>
      <td>Comedy, Drama</td>
      <td>8.0</td>
      <td>A man is embarrassed when he finds out his mot...</td>
      <td>77.97153</td>
      <td>Amit Ravindernath Sharma</td>
      <td>Ayushmann Khurrana</td>
      <td>Neena Gupta</td>
      <td>Gajraj Rao</td>
      <td>Sanya Malhotra</td>
      <td>27978</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>323</th>
      <td>Togo</td>
      <td>2019</td>
      <td>U</td>
      <td>113</td>
      <td>Adventure, Biography, Drama</td>
      <td>8.0</td>
      <td>The story of Togo, the sled dog who led the 19...</td>
      <td>69.00000</td>
      <td>Ericson Core</td>
      <td>Willem Dafoe</td>
      <td>Julianne Nicholson</td>
      <td>Christopher Heyerdahl</td>
      <td>Richard Dormer</td>
      <td>37556</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>324</th>
      <td>Airlift</td>
      <td>2016</td>
      <td>UA</td>
      <td>130</td>
      <td>Drama, History</td>
      <td>8.0</td>
      <td>When Iraq invades Kuwait in August 1990, a cal...</td>
      <td>77.97153</td>
      <td>Raja Menon</td>
      <td>Akshay Kumar</td>
      <td>Nimrat Kaur</td>
      <td>Kumud Mishra</td>
      <td>Prakash Belawadi</td>
      <td>52897</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>325</th>
      <td>Bajrangi Bhaijaan</td>
      <td>2015</td>
      <td>UA</td>
      <td>163</td>
      <td>Action, Adventure, Comedy</td>
      <td>8.0</td>
      <td>An Indian man with a magnanimous heart takes a...</td>
      <td>77.97153</td>
      <td>Kabir Khan</td>
      <td>Salman Khan</td>
      <td>Harshaali Malhotra</td>
      <td>Nawazuddin Siddiqui</td>
      <td>Kareena Kapoor</td>
      <td>72245</td>
      <td>8178001</td>
    </tr>
    <tr>
      <th>326</th>
      <td>Baby</td>
      <td>2015</td>
      <td>UA</td>
      <td>159</td>
      <td>Action, Crime, Thriller</td>
      <td>8.0</td>
      <td>An elite counter-intelligence unit learns of a...</td>
      <td>77.97153</td>
      <td>Neeraj Pandey</td>
      <td>Akshay Kumar</td>
      <td>Danny Denzongpa</td>
      <td>Rana Daggubati</td>
      <td>Taapsee Pannu</td>
      <td>52848</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>327</th>
      <td>La La Land</td>
      <td>2016</td>
      <td>A</td>
      <td>128</td>
      <td>Comedy, Drama, Music</td>
      <td>8.0</td>
      <td>While navigating their careers in Los Angeles,...</td>
      <td>94.00000</td>
      <td>Damien Chazelle</td>
      <td>Ryan Gosling</td>
      <td>Emma Stone</td>
      <td>Rosemarie DeWitt</td>
      <td>J.K. Simmons</td>
      <td>505918</td>
      <td>151101803</td>
    </tr>
    <tr>
      <th>328</th>
      <td>Lion</td>
      <td>2016</td>
      <td>U</td>
      <td>118</td>
      <td>Biography, Drama</td>
      <td>8.0</td>
      <td>A five-year-old Indian boy is adopted by an Au...</td>
      <td>69.00000</td>
      <td>Garth Davis</td>
      <td>Dev Patel</td>
      <td>Nicole Kidman</td>
      <td>Rooney Mara</td>
      <td>Sunny Pawar</td>
      <td>213970</td>
      <td>51739495</td>
    </tr>
    <tr>
      <th>329</th>
      <td>The Martian</td>
      <td>2015</td>
      <td>UA</td>
      <td>144</td>
      <td>Adventure, Drama, Sci-Fi</td>
      <td>8.0</td>
      <td>An astronaut becomes stranded on Mars after hi...</td>
      <td>80.00000</td>
      <td>Ridley Scott</td>
      <td>Matt Damon</td>
      <td>Jessica Chastain</td>
      <td>Kristen Wiig</td>
      <td>Kate Mara</td>
      <td>760094</td>
      <td>228433663</td>
    </tr>
    <tr>
      <th>330</th>
      <td>Zootopia</td>
      <td>2016</td>
      <td>U</td>
      <td>108</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.0</td>
      <td>In a city of anthropomorphic animals, a rookie...</td>
      <td>78.00000</td>
      <td>Byron Howard</td>
      <td>Rich Moore</td>
      <td>Jared Bush</td>
      <td>Ginnifer Goodwin</td>
      <td>Jason Bateman</td>
      <td>434143</td>
      <td>341268248</td>
    </tr>
    <tr>
      <th>331</th>
      <td>Bãhubali: The Beginning</td>
      <td>2015</td>
      <td>UA</td>
      <td>159</td>
      <td>Action, Drama</td>
      <td>8.0</td>
      <td>In ancient India, an adventurous and daring ma...</td>
      <td>77.97153</td>
      <td>S.S. Rajamouli</td>
      <td>Prabhas</td>
      <td>Rana Daggubati</td>
      <td>Ramya Krishnan</td>
      <td>Sathyaraj</td>
      <td>102972</td>
      <td>6738000</td>
    </tr>
    <tr>
      <th>332</th>
      <td>Kaguyahime no monogatari</td>
      <td>2013</td>
      <td>U</td>
      <td>137</td>
      <td>Animation, Adventure, Drama</td>
      <td>8.0</td>
      <td>Found inside a shining stalk of bamboo by an o...</td>
      <td>89.00000</td>
      <td>Isao Takahata</td>
      <td>Chloë Grace Moretz</td>
      <td>James Caan</td>
      <td>Mary Steenburgen</td>
      <td>James Marsden</td>
      <td>38746</td>
      <td>1506975</td>
    </tr>
    <tr>
      <th>333</th>
      <td>Wonder</td>
      <td>2017</td>
      <td>U</td>
      <td>113</td>
      <td>Drama, Family</td>
      <td>8.0</td>
      <td>Based on the New York Times bestseller, this m...</td>
      <td>66.00000</td>
      <td>Stephen Chbosky</td>
      <td>Jacob Tremblay</td>
      <td>Owen Wilson</td>
      <td>Izabela Vidovic</td>
      <td>Julia Roberts</td>
      <td>141923</td>
      <td>132422809</td>
    </tr>
    <tr>
      <th>334</th>
      <td>Gully Boy</td>
      <td>2019</td>
      <td>UA</td>
      <td>154</td>
      <td>Drama, Music, Romance</td>
      <td>8.0</td>
      <td>A coming-of-age story based on the lives of st...</td>
      <td>65.00000</td>
      <td>Zoya Akhtar</td>
      <td>Vijay Varma</td>
      <td>Nakul Roshan Sahdev</td>
      <td>Ranveer Singh</td>
      <td>Vijay Raaz</td>
      <td>31886</td>
      <td>5566534</td>
    </tr>
    <tr>
      <th>335</th>
      <td>Special Chabbis</td>
      <td>2013</td>
      <td>UA</td>
      <td>144</td>
      <td>Crime, Drama, Thriller</td>
      <td>8.0</td>
      <td>A gang of con-men rob prominent rich businessm...</td>
      <td>77.97153</td>
      <td>Neeraj Pandey</td>
      <td>Akshay Kumar</td>
      <td>Anupam Kher</td>
      <td>Manoj Bajpayee</td>
      <td>Jimmy Sheirgill</td>
      <td>51069</td>
      <td>1079369</td>
    </tr>
    <tr>
      <th>336</th>
      <td>Short Term 12</td>
      <td>2013</td>
      <td>R</td>
      <td>96</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>A 20-something supervising staff member of a r...</td>
      <td>82.00000</td>
      <td>Destin Daniel Cretton</td>
      <td>Brie Larson</td>
      <td>Frantz Turner</td>
      <td>John Gallagher Jr.</td>
      <td>Kaitlyn Dever</td>
      <td>81770</td>
      <td>1010414</td>
    </tr>
    <tr>
      <th>337</th>
      <td>Serbuan maut 2: Berandal</td>
      <td>2014</td>
      <td>A</td>
      <td>150</td>
      <td>Action, Crime, Thriller</td>
      <td>8.0</td>
      <td>Only a short time after the first raid, Rama g...</td>
      <td>71.00000</td>
      <td>Gareth Evans</td>
      <td>Iko Uwais</td>
      <td>Yayan Ruhian</td>
      <td>Arifin Putra</td>
      <td>Oka Antara</td>
      <td>114316</td>
      <td>2625803</td>
    </tr>
    <tr>
      <th>338</th>
      <td>The Imitation Game</td>
      <td>2014</td>
      <td>UA</td>
      <td>114</td>
      <td>Biography, Drama, Thriller</td>
      <td>8.0</td>
      <td>During World War II, the English mathematical ...</td>
      <td>73.00000</td>
      <td>Morten Tyldum</td>
      <td>Benedict Cumberbatch</td>
      <td>Keira Knightley</td>
      <td>Matthew Goode</td>
      <td>Allen Leech</td>
      <td>685201</td>
      <td>91125683</td>
    </tr>
    <tr>
      <th>339</th>
      <td>Guardians of the Galaxy</td>
      <td>2014</td>
      <td>UA</td>
      <td>121</td>
      <td>Action, Adventure, Comedy</td>
      <td>8.0</td>
      <td>A group of intergalactic criminals must pull t...</td>
      <td>76.00000</td>
      <td>James Gunn</td>
      <td>Chris Pratt</td>
      <td>Vin Diesel</td>
      <td>Bradley Cooper</td>
      <td>Zoe Saldana</td>
      <td>1043455</td>
      <td>333176600</td>
    </tr>
    <tr>
      <th>340</th>
      <td>Blade Runner 2049</td>
      <td>2017</td>
      <td>UA</td>
      <td>164</td>
      <td>Action, Drama, Mystery</td>
      <td>8.0</td>
      <td>Young Blade Runner K's discovery of a long-bur...</td>
      <td>81.00000</td>
      <td>Denis Villeneuve</td>
      <td>Harrison Ford</td>
      <td>Ryan Gosling</td>
      <td>Ana de Armas</td>
      <td>Dave Bautista</td>
      <td>461823</td>
      <td>92054159</td>
    </tr>
    <tr>
      <th>341</th>
      <td>Her</td>
      <td>2013</td>
      <td>A</td>
      <td>126</td>
      <td>Drama, Romance, Sci-Fi</td>
      <td>8.0</td>
      <td>In a near future, a lonely writer develops an ...</td>
      <td>90.00000</td>
      <td>Spike Jonze</td>
      <td>Joaquin Phoenix</td>
      <td>Amy Adams</td>
      <td>Scarlett Johansson</td>
      <td>Rooney Mara</td>
      <td>540772</td>
      <td>25568251</td>
    </tr>
    <tr>
      <th>342</th>
      <td>Bohemian Rhapsody</td>
      <td>2018</td>
      <td>UA</td>
      <td>134</td>
      <td>Biography, Drama, Music</td>
      <td>8.0</td>
      <td>The story of the legendary British rock band Q...</td>
      <td>49.00000</td>
      <td>Bryan Singer</td>
      <td>Rami Malek</td>
      <td>Lucy Boynton</td>
      <td>Gwilym Lee</td>
      <td>Ben Hardy</td>
      <td>450349</td>
      <td>216428042</td>
    </tr>
    <tr>
      <th>343</th>
      <td>The Revenant</td>
      <td>2015</td>
      <td>A</td>
      <td>156</td>
      <td>Action, Adventure, Drama</td>
      <td>8.0</td>
      <td>A frontiersman on a fur trading expedition in ...</td>
      <td>76.00000</td>
      <td>Alejandro G. Iñárritu</td>
      <td>Leonardo DiCaprio</td>
      <td>Tom Hardy</td>
      <td>Will Poulter</td>
      <td>Domhnall Gleeson</td>
      <td>705589</td>
      <td>183637894</td>
    </tr>
    <tr>
      <th>344</th>
      <td>The Perks of Being a Wallflower</td>
      <td>2012</td>
      <td>UA</td>
      <td>103</td>
      <td>Drama, Romance</td>
      <td>8.0</td>
      <td>An introvert freshman is taken under the wings...</td>
      <td>67.00000</td>
      <td>Stephen Chbosky</td>
      <td>Logan Lerman</td>
      <td>Emma Watson</td>
      <td>Ezra Miller</td>
      <td>Paul Rudd</td>
      <td>462252</td>
      <td>17738570</td>
    </tr>
    <tr>
      <th>345</th>
      <td>Tropa de Elite 2: O Inimigo Agora é Outro</td>
      <td>2010</td>
      <td>Unknown</td>
      <td>115</td>
      <td>Action, Crime, Drama</td>
      <td>8.0</td>
      <td>After a prison riot, former-Captain Nascimento...</td>
      <td>71.00000</td>
      <td>José Padilha</td>
      <td>Wagner Moura</td>
      <td>Irandhir Santos</td>
      <td>André Ramiro</td>
      <td>Milhem Cortaz</td>
      <td>79200</td>
      <td>100119</td>
    </tr>
    <tr>
      <th>346</th>
      <td>The King's Speech</td>
      <td>2010</td>
      <td>U</td>
      <td>118</td>
      <td>Biography, Drama, History</td>
      <td>8.0</td>
      <td>The story of King George VI, his impromptu asc...</td>
      <td>88.00000</td>
      <td>Tom Hooper</td>
      <td>Colin Firth</td>
      <td>Geoffrey Rush</td>
      <td>Helena Bonham Carter</td>
      <td>Derek Jacobi</td>
      <td>639603</td>
      <td>138797449</td>
    </tr>
    <tr>
      <th>347</th>
      <td>The Help</td>
      <td>2011</td>
      <td>UA</td>
      <td>146</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>An aspiring author during the civil rights mov...</td>
      <td>62.00000</td>
      <td>Tate Taylor</td>
      <td>Emma Stone</td>
      <td>Viola Davis</td>
      <td>Octavia Spencer</td>
      <td>Bryce Dallas Howard</td>
      <td>428521</td>
      <td>169708112</td>
    </tr>
    <tr>
      <th>348</th>
      <td>Deadpool</td>
      <td>2016</td>
      <td>R</td>
      <td>108</td>
      <td>Action, Adventure, Comedy</td>
      <td>8.0</td>
      <td>A wisecracking mercenary gets experimented on ...</td>
      <td>65.00000</td>
      <td>Tim Miller</td>
      <td>Ryan Reynolds</td>
      <td>Morena Baccarin</td>
      <td>T.J. Miller</td>
      <td>Ed Skrein</td>
      <td>902669</td>
      <td>363070709</td>
    </tr>
    <tr>
      <th>349</th>
      <td>Darbareye Elly</td>
      <td>2009</td>
      <td>TV-PG</td>
      <td>119</td>
      <td>Drama, Mystery</td>
      <td>8.0</td>
      <td>The mysterious disappearance of a kindergarten...</td>
      <td>87.00000</td>
      <td>Asghar Farhadi</td>
      <td>Golshifteh Farahani</td>
      <td>Shahab Hosseini</td>
      <td>Taraneh Alidoosti</td>
      <td>Merila Zare'i</td>
      <td>45803</td>
      <td>106662</td>
    </tr>
    <tr>
      <th>350</th>
      <td>Dev.D</td>
      <td>2009</td>
      <td>A</td>
      <td>144</td>
      <td>Drama, Romance</td>
      <td>8.0</td>
      <td>After breaking up with his childhood sweethear...</td>
      <td>77.97153</td>
      <td>Anurag Kashyap</td>
      <td>Abhay Deol</td>
      <td>Mahie Gill</td>
      <td>Kalki Koechlin</td>
      <td>Dibyendu Bhattacharya</td>
      <td>28749</td>
      <td>10950</td>
    </tr>
    <tr>
      <th>351</th>
      <td>Yip Man</td>
      <td>2008</td>
      <td>R</td>
      <td>106</td>
      <td>Action, Biography, Drama</td>
      <td>8.0</td>
      <td>During the Japanese invasion of China, a wealt...</td>
      <td>59.00000</td>
      <td>Wilson Yip</td>
      <td>Donnie Yen</td>
      <td>Simon Yam</td>
      <td>Siu-Wong Fan</td>
      <td>Ka Tung Lam</td>
      <td>211427</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>352</th>
      <td>My Name Is Khan</td>
      <td>2010</td>
      <td>UA</td>
      <td>165</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>An Indian Muslim man with Asperger's syndrome ...</td>
      <td>50.00000</td>
      <td>Karan Johar</td>
      <td>Shah Rukh Khan</td>
      <td>Kajol</td>
      <td>Sheetal Menon</td>
      <td>Katie A. Keane</td>
      <td>98575</td>
      <td>4018695</td>
    </tr>
    <tr>
      <th>353</th>
      <td>Nefes: Vatan Sagolsun</td>
      <td>2009</td>
      <td>Unknown</td>
      <td>128</td>
      <td>Action, Drama, Thriller</td>
      <td>8.0</td>
      <td>Story of 40-man Turkish task force who must de...</td>
      <td>77.97153</td>
      <td>Levent Semerci</td>
      <td>Erdem Can</td>
      <td>Mete Horozoglu</td>
      <td>Ilker Kizmaz</td>
      <td>Baris Bagci</td>
      <td>31838</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>354</th>
      <td>Slumdog Millionaire</td>
      <td>2008</td>
      <td>UA</td>
      <td>120</td>
      <td>Drama, Romance</td>
      <td>8.0</td>
      <td>A Mumbai teenager reflects on his life after b...</td>
      <td>84.00000</td>
      <td>Danny Boyle</td>
      <td>Loveleen Tandan</td>
      <td>Dev Patel</td>
      <td>Freida Pinto</td>
      <td>Saurabh Shukla</td>
      <td>798882</td>
      <td>141319928</td>
    </tr>
    <tr>
      <th>355</th>
      <td>Black Swan</td>
      <td>2010</td>
      <td>A</td>
      <td>108</td>
      <td>Drama, Thriller</td>
      <td>8.0</td>
      <td>A committed dancer struggles to maintain her s...</td>
      <td>79.00000</td>
      <td>Darren Aronofsky</td>
      <td>Natalie Portman</td>
      <td>Mila Kunis</td>
      <td>Vincent Cassel</td>
      <td>Winona Ryder</td>
      <td>699673</td>
      <td>106954678</td>
    </tr>
    <tr>
      <th>356</th>
      <td>Tropa de Elite</td>
      <td>2007</td>
      <td>R</td>
      <td>115</td>
      <td>Action, Crime, Drama</td>
      <td>8.0</td>
      <td>In 1997 Rio de Janeiro, Captain Nascimento has...</td>
      <td>33.00000</td>
      <td>José Padilha</td>
      <td>Wagner Moura</td>
      <td>André Ramiro</td>
      <td>Caio Junqueira</td>
      <td>Milhem Cortaz</td>
      <td>98097</td>
      <td>8060</td>
    </tr>
    <tr>
      <th>357</th>
      <td>The Avengers</td>
      <td>2012</td>
      <td>UA</td>
      <td>143</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>8.0</td>
      <td>Earth's mightiest heroes must come together an...</td>
      <td>69.00000</td>
      <td>Joss Whedon</td>
      <td>Robert Downey Jr.</td>
      <td>Chris Evans</td>
      <td>Scarlett Johansson</td>
      <td>Jeremy Renner</td>
      <td>1260806</td>
      <td>623279547</td>
    </tr>
    <tr>
      <th>358</th>
      <td>Persepolis</td>
      <td>2007</td>
      <td>PG-13</td>
      <td>96</td>
      <td>Animation, Biography, Drama</td>
      <td>8.0</td>
      <td>A precocious and outspoken Iranian girl grows ...</td>
      <td>90.00000</td>
      <td>Vincent Paronnaud</td>
      <td>Marjane Satrapi</td>
      <td>Chiara Mastroianni</td>
      <td>Catherine Deneuve</td>
      <td>Gena Rowlands</td>
      <td>88656</td>
      <td>4445756</td>
    </tr>
    <tr>
      <th>359</th>
      <td>Dallas Buyers Club</td>
      <td>2013</td>
      <td>R</td>
      <td>117</td>
      <td>Biography, Drama</td>
      <td>8.0</td>
      <td>In 1985 Dallas, electrician and hustler Ron Wo...</td>
      <td>80.00000</td>
      <td>Jean-Marc Vallée</td>
      <td>Matthew McConaughey</td>
      <td>Jennifer Garner</td>
      <td>Jared Leto</td>
      <td>Steve Zahn</td>
      <td>441614</td>
      <td>27298285</td>
    </tr>
    <tr>
      <th>360</th>
      <td>The Pursuit of Happyness</td>
      <td>2006</td>
      <td>U</td>
      <td>117</td>
      <td>Biography, Drama</td>
      <td>8.0</td>
      <td>A struggling salesman takes custody of his son...</td>
      <td>64.00000</td>
      <td>Gabriele Muccino</td>
      <td>Will Smith</td>
      <td>Thandie Newton</td>
      <td>Jaden Smith</td>
      <td>Brian Howe</td>
      <td>448930</td>
      <td>163566459</td>
    </tr>
    <tr>
      <th>361</th>
      <td>Blood Diamond</td>
      <td>2006</td>
      <td>A</td>
      <td>143</td>
      <td>Adventure, Drama, Thriller</td>
      <td>8.0</td>
      <td>A fisherman, a smuggler, and a syndicate of bu...</td>
      <td>64.00000</td>
      <td>Edward Zwick</td>
      <td>Leonardo DiCaprio</td>
      <td>Djimon Hounsou</td>
      <td>Jennifer Connelly</td>
      <td>Kagiso Kuypers</td>
      <td>499439</td>
      <td>57366262</td>
    </tr>
    <tr>
      <th>362</th>
      <td>The Bourne Ultimatum</td>
      <td>2007</td>
      <td>UA</td>
      <td>115</td>
      <td>Action, Mystery, Thriller</td>
      <td>8.0</td>
      <td>Jason Bourne dodges a ruthless C.I.A. official...</td>
      <td>85.00000</td>
      <td>Paul Greengrass</td>
      <td>Matt Damon</td>
      <td>Edgar Ramírez</td>
      <td>Joan Allen</td>
      <td>Julia Stiles</td>
      <td>604694</td>
      <td>227471070</td>
    </tr>
    <tr>
      <th>363</th>
      <td>Bin-jip</td>
      <td>2004</td>
      <td>U</td>
      <td>88</td>
      <td>Crime, Drama, Romance</td>
      <td>8.0</td>
      <td>A transient young man breaks into empty homes ...</td>
      <td>72.00000</td>
      <td>Ki-duk Kim</td>
      <td>Seung-Yun Lee</td>
      <td>Hee Jae</td>
      <td>Hyuk-ho Kwon</td>
      <td>Jin-mo Joo</td>
      <td>50610</td>
      <td>238507</td>
    </tr>
    <tr>
      <th>364</th>
      <td>Sin City</td>
      <td>2005</td>
      <td>A</td>
      <td>124</td>
      <td>Crime, Thriller</td>
      <td>8.0</td>
      <td>A movie that explores the dark and miserable t...</td>
      <td>74.00000</td>
      <td>Frank Miller</td>
      <td>Quentin Tarantino</td>
      <td>Robert Rodriguez</td>
      <td>Mickey Rourke</td>
      <td>Clive Owen</td>
      <td>738512</td>
      <td>74103820</td>
    </tr>
    <tr>
      <th>365</th>
      <td>Le scaphandre et le papillon</td>
      <td>2007</td>
      <td>PG-13</td>
      <td>112</td>
      <td>Biography, Drama</td>
      <td>8.0</td>
      <td>The true story of Elle editor Jean-Dominique B...</td>
      <td>92.00000</td>
      <td>Julian Schnabel</td>
      <td>Laura Obiols</td>
      <td>Mathieu Amalric</td>
      <td>Emmanuelle Seigner</td>
      <td>Marie-Josée Croze</td>
      <td>103284</td>
      <td>5990075</td>
    </tr>
    <tr>
      <th>366</th>
      <td>G.O.R.A.</td>
      <td>2004</td>
      <td>Unknown</td>
      <td>127</td>
      <td>Adventure, Comedy, Sci-Fi</td>
      <td>8.0</td>
      <td>A slick young Turk kidnapped by extraterrestri...</td>
      <td>77.97153</td>
      <td>Ömer Faruk Sorak</td>
      <td>Cem Yilmaz</td>
      <td>Özge Özberk</td>
      <td>Ozan Güven</td>
      <td>Safak Sezer</td>
      <td>56960</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>367</th>
      <td>Ratatouille</td>
      <td>2007</td>
      <td>U</td>
      <td>111</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.0</td>
      <td>A rat who can cook makes an unusual alliance w...</td>
      <td>96.00000</td>
      <td>Brad Bird</td>
      <td>Jan Pinkava</td>
      <td>Brad Garrett</td>
      <td>Lou Romano</td>
      <td>Patton Oswalt</td>
      <td>641645</td>
      <td>206445654</td>
    </tr>
    <tr>
      <th>368</th>
      <td>Casino Royale</td>
      <td>2006</td>
      <td>PG-13</td>
      <td>144</td>
      <td>Action, Adventure, Thriller</td>
      <td>8.0</td>
      <td>After earning 00 status and a licence to kill,...</td>
      <td>80.00000</td>
      <td>Martin Campbell</td>
      <td>Daniel Craig</td>
      <td>Eva Green</td>
      <td>Judi Dench</td>
      <td>Jeffrey Wright</td>
      <td>582239</td>
      <td>167445960</td>
    </tr>
    <tr>
      <th>369</th>
      <td>Kill Bill: Vol. 2</td>
      <td>2004</td>
      <td>A</td>
      <td>137</td>
      <td>Action, Crime, Thriller</td>
      <td>8.0</td>
      <td>The Bride continues her quest of vengeance aga...</td>
      <td>83.00000</td>
      <td>Quentin Tarantino</td>
      <td>Uma Thurman</td>
      <td>David Carradine</td>
      <td>Michael Madsen</td>
      <td>Daryl Hannah</td>
      <td>683900</td>
      <td>66208183</td>
    </tr>
    <tr>
      <th>370</th>
      <td>Vozvrashchenie</td>
      <td>2003</td>
      <td>Unknown</td>
      <td>110</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>In the Russian wilderness, two brothers face a...</td>
      <td>82.00000</td>
      <td>Andrey Zvyagintsev</td>
      <td>Vladimir Garin</td>
      <td>Ivan Dobronravov</td>
      <td>Konstantin Lavronenko</td>
      <td>Nataliya Vdovina</td>
      <td>42399</td>
      <td>502028</td>
    </tr>
    <tr>
      <th>371</th>
      <td>Bom Yeoareum Gaeul Gyeoul Geurigo Bom</td>
      <td>2003</td>
      <td>R</td>
      <td>103</td>
      <td>Drama, Romance</td>
      <td>8.0</td>
      <td>A boy is raised by a Buddhist monk in an isola...</td>
      <td>85.00000</td>
      <td>Ki-duk Kim</td>
      <td>Ki-duk Kim</td>
      <td>Yeong-su Oh</td>
      <td>Jong-ho Kim</td>
      <td>Kim Young-Min</td>
      <td>77520</td>
      <td>2380788</td>
    </tr>
    <tr>
      <th>372</th>
      <td>Mar adentro</td>
      <td>2014</td>
      <td>U</td>
      <td>126</td>
      <td>Biography, Drama</td>
      <td>8.0</td>
      <td>The factual story of Spaniard Ramon Sampedro, ...</td>
      <td>74.00000</td>
      <td>Alejandro Amenábar</td>
      <td>Javier Bardem</td>
      <td>Belén Rueda</td>
      <td>Lola Dueñas</td>
      <td>Mabel Rivera</td>
      <td>77554</td>
      <td>2086345</td>
    </tr>
    <tr>
      <th>373</th>
      <td>Cinderella Man</td>
      <td>2005</td>
      <td>UA</td>
      <td>144</td>
      <td>Biography, Drama, History</td>
      <td>8.0</td>
      <td>The story of James J. Braddock, a supposedly w...</td>
      <td>69.00000</td>
      <td>Ron Howard</td>
      <td>Russell Crowe</td>
      <td>Renée Zellweger</td>
      <td>Craig Bierko</td>
      <td>Paul Giamatti</td>
      <td>176151</td>
      <td>61649911</td>
    </tr>
    <tr>
      <th>374</th>
      <td>Kal Ho Naa Ho</td>
      <td>2003</td>
      <td>U</td>
      <td>186</td>
      <td>Comedy, Drama, Musical</td>
      <td>8.0</td>
      <td>Naina, an introverted, perpetually depressed g...</td>
      <td>54.00000</td>
      <td>Nikkhil Advani</td>
      <td>Preity Zinta</td>
      <td>Shah Rukh Khan</td>
      <td>Saif Ali Khan</td>
      <td>Jaya Bachchan</td>
      <td>63460</td>
      <td>1787378</td>
    </tr>
    <tr>
      <th>375</th>
      <td>Mou gaan dou</td>
      <td>2002</td>
      <td>UA</td>
      <td>101</td>
      <td>Action, Crime, Drama</td>
      <td>8.0</td>
      <td>A story between a mole in the police departmen...</td>
      <td>75.00000</td>
      <td>Andrew Lau</td>
      <td>Alan Mak</td>
      <td>Andy Lau</td>
      <td>Tony Chiu-Wai Leung</td>
      <td>Anthony Chau-Sang Wong</td>
      <td>117857</td>
      <td>169659</td>
    </tr>
    <tr>
      <th>376</th>
      <td>Pirates of the Caribbean: The Curse of the Bla...</td>
      <td>2003</td>
      <td>UA</td>
      <td>143</td>
      <td>Action, Adventure, Fantasy</td>
      <td>8.0</td>
      <td>Blacksmith Will Turner teams up with eccentric...</td>
      <td>63.00000</td>
      <td>Gore Verbinski</td>
      <td>Johnny Depp</td>
      <td>Geoffrey Rush</td>
      <td>Orlando Bloom</td>
      <td>Keira Knightley</td>
      <td>1015122</td>
      <td>305413918</td>
    </tr>
    <tr>
      <th>377</th>
      <td>Big Fish</td>
      <td>2003</td>
      <td>U</td>
      <td>125</td>
      <td>Adventure, Drama, Fantasy</td>
      <td>8.0</td>
      <td>A frustrated son tries to determine the fact f...</td>
      <td>58.00000</td>
      <td>Tim Burton</td>
      <td>Ewan McGregor</td>
      <td>Albert Finney</td>
      <td>Billy Crudup</td>
      <td>Jessica Lange</td>
      <td>415218</td>
      <td>66257002</td>
    </tr>
    <tr>
      <th>378</th>
      <td>The Incredibles</td>
      <td>2004</td>
      <td>U</td>
      <td>115</td>
      <td>Animation, Action, Adventure</td>
      <td>8.0</td>
      <td>A family of undercover superheroes, while tryi...</td>
      <td>90.00000</td>
      <td>Brad Bird</td>
      <td>Craig T. Nelson</td>
      <td>Samuel L. Jackson</td>
      <td>Holly Hunter</td>
      <td>Jason Lee</td>
      <td>657047</td>
      <td>261441092</td>
    </tr>
    <tr>
      <th>379</th>
      <td>Yeopgijeogin geunyeo</td>
      <td>2001</td>
      <td>Unknown</td>
      <td>137</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.0</td>
      <td>A young man sees a drunk, cute woman standing ...</td>
      <td>77.97153</td>
      <td>Jae-young Kwak</td>
      <td>Tae-Hyun Cha</td>
      <td>Jun Ji-Hyun</td>
      <td>In-mun Kim</td>
      <td>Song Wok-suk</td>
      <td>45403</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>380</th>
      <td>Dogville</td>
      <td>2003</td>
      <td>R</td>
      <td>178</td>
      <td>Crime, Drama</td>
      <td>8.0</td>
      <td>A woman on the run from the mob is reluctantly...</td>
      <td>60.00000</td>
      <td>Lars von Trier</td>
      <td>Nicole Kidman</td>
      <td>Paul Bettany</td>
      <td>Lauren Bacall</td>
      <td>Harriet Andersson</td>
      <td>137963</td>
      <td>1530386</td>
    </tr>
    <tr>
      <th>381</th>
      <td>Vizontele</td>
      <td>2001</td>
      <td>Unknown</td>
      <td>110</td>
      <td>Comedy, Drama</td>
      <td>8.0</td>
      <td>Lives of residents in a small Anatolian villag...</td>
      <td>77.97153</td>
      <td>Yilmaz Erdogan</td>
      <td>Ömer Faruk Sorak</td>
      <td>Yilmaz Erdogan</td>
      <td>Demet Akbag</td>
      <td>Altan Erkekli</td>
      <td>33592</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>382</th>
      <td>Donnie Darko</td>
      <td>2001</td>
      <td>R</td>
      <td>113</td>
      <td>Drama, Mystery, Sci-Fi</td>
      <td>8.0</td>
      <td>After narrowly escaping a bizarre accident, a ...</td>
      <td>88.00000</td>
      <td>Richard Kelly</td>
      <td>Jake Gyllenhaal</td>
      <td>Jena Malone</td>
      <td>Mary McDonnell</td>
      <td>Holmes Osborne</td>
      <td>740086</td>
      <td>1480006</td>
    </tr>
    <tr>
      <th>383</th>
      <td>Magnolia</td>
      <td>1999</td>
      <td>R</td>
      <td>188</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>An epic mosaic of interrelated characters in s...</td>
      <td>77.00000</td>
      <td>Paul Thomas Anderson</td>
      <td>Tom Cruise</td>
      <td>Jason Robards</td>
      <td>Julianne Moore</td>
      <td>Philip Seymour Hoffman</td>
      <td>289742</td>
      <td>22455976</td>
    </tr>
    <tr>
      <th>384</th>
      <td>Dancer in the Dark</td>
      <td>2000</td>
      <td>U</td>
      <td>140</td>
      <td>Crime, Drama, Musical</td>
      <td>8.0</td>
      <td>An East European girl travels to the United St...</td>
      <td>61.00000</td>
      <td>Lars von Trier</td>
      <td>Björk</td>
      <td>Catherine Deneuve</td>
      <td>David Morse</td>
      <td>Peter Stormare</td>
      <td>102285</td>
      <td>4184036</td>
    </tr>
    <tr>
      <th>385</th>
      <td>The Straight Story</td>
      <td>1999</td>
      <td>U</td>
      <td>112</td>
      <td>Biography, Drama</td>
      <td>8.0</td>
      <td>An old man makes a long journey by lawnmower t...</td>
      <td>86.00000</td>
      <td>David Lynch</td>
      <td>Richard Farnsworth</td>
      <td>Sissy Spacek</td>
      <td>Jane Galloway Heitz</td>
      <td>Joseph A. Carpenter</td>
      <td>82002</td>
      <td>6203044</td>
    </tr>
    <tr>
      <th>386</th>
      <td>Pâfekuto burû</td>
      <td>1997</td>
      <td>A</td>
      <td>81</td>
      <td>Animation, Crime, Mystery</td>
      <td>8.0</td>
      <td>A pop singer gives up her career to become an ...</td>
      <td>77.97153</td>
      <td>Satoshi Kon</td>
      <td>Junko Iwao</td>
      <td>Rica Matsumoto</td>
      <td>Shinpachi Tsuji</td>
      <td>Masaaki Ôkura</td>
      <td>58192</td>
      <td>776665</td>
    </tr>
    <tr>
      <th>387</th>
      <td>Festen</td>
      <td>1998</td>
      <td>R</td>
      <td>105</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>At Helge's 60th birthday party, some unpleasan...</td>
      <td>82.00000</td>
      <td>Thomas Vinterberg</td>
      <td>Ulrich Thomsen</td>
      <td>Henning Moritzen</td>
      <td>Thomas Bo Larsen</td>
      <td>Paprika Steen</td>
      <td>78341</td>
      <td>1647780</td>
    </tr>
    <tr>
      <th>388</th>
      <td>Central do Brasil</td>
      <td>1998</td>
      <td>R</td>
      <td>110</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>An emotive journey of a former school teacher,...</td>
      <td>80.00000</td>
      <td>Walter Salles</td>
      <td>Fernanda Montenegro</td>
      <td>Vinícius de Oliveira</td>
      <td>Marília Pêra</td>
      <td>Soia Lira</td>
      <td>36419</td>
      <td>5595428</td>
    </tr>
    <tr>
      <th>389</th>
      <td>The Iron Giant</td>
      <td>1999</td>
      <td>PG</td>
      <td>86</td>
      <td>Animation, Action, Adventure</td>
      <td>8.0</td>
      <td>A young boy befriends a giant robot from outer...</td>
      <td>85.00000</td>
      <td>Brad Bird</td>
      <td>Eli Marienthal</td>
      <td>Harry Connick Jr.</td>
      <td>Jennifer Aniston</td>
      <td>Vin Diesel</td>
      <td>172083</td>
      <td>23159305</td>
    </tr>
    <tr>
      <th>390</th>
      <td>Knockin' on Heaven's Door</td>
      <td>1997</td>
      <td>Unknown</td>
      <td>87</td>
      <td>Action, Crime, Comedy</td>
      <td>8.0</td>
      <td>Two terminally ill patients escape from a hosp...</td>
      <td>77.97153</td>
      <td>Thomas Jahn</td>
      <td>Til Schweiger</td>
      <td>Jan Josef Liefers</td>
      <td>Thierry van Werveke</td>
      <td>Moritz Bleibtreu</td>
      <td>27721</td>
      <td>3296</td>
    </tr>
    <tr>
      <th>391</th>
      <td>Sling Blade</td>
      <td>1996</td>
      <td>R</td>
      <td>135</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>Karl Childers, a simple man hospitalized since...</td>
      <td>84.00000</td>
      <td>Billy Bob Thornton</td>
      <td>Billy Bob Thornton</td>
      <td>Dwight Yoakam</td>
      <td>J.T. Walsh</td>
      <td>John Ritter</td>
      <td>86838</td>
      <td>24475416</td>
    </tr>
    <tr>
      <th>392</th>
      <td>Secrets &amp; Lies</td>
      <td>1996</td>
      <td>U</td>
      <td>136</td>
      <td>Comedy, Drama</td>
      <td>8.0</td>
      <td>Following the death of her adoptive parents, a...</td>
      <td>91.00000</td>
      <td>Mike Leigh</td>
      <td>Timothy Spall</td>
      <td>Brenda Blethyn</td>
      <td>Phyllis Logan</td>
      <td>Claire Rushbrook</td>
      <td>37564</td>
      <td>13417292</td>
    </tr>
    <tr>
      <th>393</th>
      <td>Twelve Monkeys</td>
      <td>1995</td>
      <td>A</td>
      <td>129</td>
      <td>Mystery, Sci-Fi, Thriller</td>
      <td>8.0</td>
      <td>In a future world devastated by disease, a con...</td>
      <td>74.00000</td>
      <td>Terry Gilliam</td>
      <td>Bruce Willis</td>
      <td>Madeleine Stowe</td>
      <td>Brad Pitt</td>
      <td>Joseph Melito</td>
      <td>578443</td>
      <td>57141459</td>
    </tr>
    <tr>
      <th>394</th>
      <td>Kôkaku Kidôtai</td>
      <td>1995</td>
      <td>UA</td>
      <td>83</td>
      <td>Animation, Action, Crime</td>
      <td>8.0</td>
      <td>A cyborg policewoman and her partner hunt a my...</td>
      <td>76.00000</td>
      <td>Mamoru Oshii</td>
      <td>Atsuko Tanaka</td>
      <td>Iemasa Kayumi</td>
      <td>Akio Ôtsuka</td>
      <td>Kôichi Yamadera</td>
      <td>129231</td>
      <td>515905</td>
    </tr>
    <tr>
      <th>395</th>
      <td>The Nightmare Before Christmas</td>
      <td>1993</td>
      <td>U</td>
      <td>76</td>
      <td>Animation, Family, Fantasy</td>
      <td>8.0</td>
      <td>Jack Skellington, king of Halloween Town, disc...</td>
      <td>82.00000</td>
      <td>Henry Selick</td>
      <td>Danny Elfman</td>
      <td>Chris Sarandon</td>
      <td>Catherine O'Hara</td>
      <td>William Hickey</td>
      <td>300208</td>
      <td>75082668</td>
    </tr>
    <tr>
      <th>396</th>
      <td>Groundhog Day</td>
      <td>1993</td>
      <td>U</td>
      <td>101</td>
      <td>Comedy, Fantasy, Romance</td>
      <td>8.0</td>
      <td>A weatherman finds himself inexplicably living...</td>
      <td>72.00000</td>
      <td>Harold Ramis</td>
      <td>Bill Murray</td>
      <td>Andie MacDowell</td>
      <td>Chris Elliott</td>
      <td>Stephen Tobolowsky</td>
      <td>577991</td>
      <td>70906973</td>
    </tr>
    <tr>
      <th>397</th>
      <td>Bound by Honor</td>
      <td>1993</td>
      <td>R</td>
      <td>180</td>
      <td>Crime, Drama</td>
      <td>8.0</td>
      <td>Based on the true life experiences of poet Jim...</td>
      <td>47.00000</td>
      <td>Taylor Hackford</td>
      <td>Damian Chapa</td>
      <td>Jesse Borrego</td>
      <td>Benjamin Bratt</td>
      <td>Enrique Castillo</td>
      <td>28825</td>
      <td>4496583</td>
    </tr>
    <tr>
      <th>398</th>
      <td>Scent of a Woman</td>
      <td>1992</td>
      <td>UA</td>
      <td>156</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>A prep school student needing money agrees to ...</td>
      <td>59.00000</td>
      <td>Martin Brest</td>
      <td>Al Pacino</td>
      <td>Chris O'Donnell</td>
      <td>James Rebhorn</td>
      <td>Gabrielle Anwar</td>
      <td>263918</td>
      <td>63895607</td>
    </tr>
    <tr>
      <th>399</th>
      <td>Aladdin</td>
      <td>1992</td>
      <td>U</td>
      <td>90</td>
      <td>Animation, Adventure, Comedy</td>
      <td>8.0</td>
      <td>A kindhearted street urchin and a power-hungry...</td>
      <td>86.00000</td>
      <td>Ron Clements</td>
      <td>John Musker</td>
      <td>Scott Weinger</td>
      <td>Robin Williams</td>
      <td>Linda Larkin</td>
      <td>373845</td>
      <td>217350219</td>
    </tr>
    <tr>
      <th>400</th>
      <td>JFK</td>
      <td>1991</td>
      <td>UA</td>
      <td>189</td>
      <td>Drama, History, Thriller</td>
      <td>8.0</td>
      <td>New Orleans District Attorney Jim Garrison dis...</td>
      <td>72.00000</td>
      <td>Oliver Stone</td>
      <td>Kevin Costner</td>
      <td>Gary Oldman</td>
      <td>Jack Lemmon</td>
      <td>Walter Matthau</td>
      <td>142110</td>
      <td>70405498</td>
    </tr>
    <tr>
      <th>401</th>
      <td>Beauty and the Beast</td>
      <td>1991</td>
      <td>G</td>
      <td>84</td>
      <td>Animation, Family, Fantasy</td>
      <td>8.0</td>
      <td>A prince cursed to spend his days as a hideous...</td>
      <td>95.00000</td>
      <td>Gary Trousdale</td>
      <td>Kirk Wise</td>
      <td>Paige O'Hara</td>
      <td>Robby Benson</td>
      <td>Jesse Corti</td>
      <td>417178</td>
      <td>218967620</td>
    </tr>
    <tr>
      <th>402</th>
      <td>Dances with Wolves</td>
      <td>1990</td>
      <td>U</td>
      <td>181</td>
      <td>Adventure, Drama, Western</td>
      <td>8.0</td>
      <td>Lieutenant John Dunbar, assigned to a remote w...</td>
      <td>72.00000</td>
      <td>Kevin Costner</td>
      <td>Kevin Costner</td>
      <td>Mary McDonnell</td>
      <td>Graham Greene</td>
      <td>Rodney A. Grant</td>
      <td>240266</td>
      <td>184208848</td>
    </tr>
    <tr>
      <th>403</th>
      <td>Do the Right Thing</td>
      <td>1989</td>
      <td>R</td>
      <td>120</td>
      <td>Comedy, Drama</td>
      <td>8.0</td>
      <td>On the hottest day of the year on a street in ...</td>
      <td>93.00000</td>
      <td>Spike Lee</td>
      <td>Danny Aiello</td>
      <td>Ossie Davis</td>
      <td>Ruby Dee</td>
      <td>Richard Edson</td>
      <td>89429</td>
      <td>27545445</td>
    </tr>
    <tr>
      <th>404</th>
      <td>Rain Man</td>
      <td>1988</td>
      <td>U</td>
      <td>133</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>Selfish yuppie Charlie Babbitt's father left a...</td>
      <td>65.00000</td>
      <td>Barry Levinson</td>
      <td>Dustin Hoffman</td>
      <td>Tom Cruise</td>
      <td>Valeria Golino</td>
      <td>Gerald R. Molen</td>
      <td>473064</td>
      <td>178800000</td>
    </tr>
    <tr>
      <th>405</th>
      <td>Akira</td>
      <td>1988</td>
      <td>UA</td>
      <td>124</td>
      <td>Animation, Action, Sci-Fi</td>
      <td>8.0</td>
      <td>A secret military project endangers Neo-Tokyo ...</td>
      <td>77.97153</td>
      <td>Katsuhiro Ôtomo</td>
      <td>Mitsuo Iwata</td>
      <td>Nozomu Sasaki</td>
      <td>Mami Koyama</td>
      <td>Tesshô Genda</td>
      <td>164918</td>
      <td>553171</td>
    </tr>
    <tr>
      <th>406</th>
      <td>The Princess Bride</td>
      <td>1987</td>
      <td>U</td>
      <td>98</td>
      <td>Adventure, Family, Fantasy</td>
      <td>8.0</td>
      <td>While home sick in bed, a young boy's grandfat...</td>
      <td>77.00000</td>
      <td>Rob Reiner</td>
      <td>Cary Elwes</td>
      <td>Mandy Patinkin</td>
      <td>Robin Wright</td>
      <td>Chris Sarandon</td>
      <td>393899</td>
      <td>30857814</td>
    </tr>
    <tr>
      <th>407</th>
      <td>Der Himmel über Berlin</td>
      <td>1987</td>
      <td>U</td>
      <td>128</td>
      <td>Drama, Fantasy, Romance</td>
      <td>8.0</td>
      <td>An angel tires of overseeing human activity an...</td>
      <td>79.00000</td>
      <td>Wim Wenders</td>
      <td>Bruno Ganz</td>
      <td>Solveig Dommartin</td>
      <td>Otto Sander</td>
      <td>Curt Bois</td>
      <td>64722</td>
      <td>3333969</td>
    </tr>
    <tr>
      <th>408</th>
      <td>Au revoir les enfants</td>
      <td>1987</td>
      <td>U</td>
      <td>104</td>
      <td>Drama, War</td>
      <td>8.0</td>
      <td>A French boarding school run by priests seems ...</td>
      <td>88.00000</td>
      <td>Louis Malle</td>
      <td>Gaspard Manesse</td>
      <td>Raphael Fejtö</td>
      <td>Francine Racette</td>
      <td>Stanislas Carré de Malberg</td>
      <td>31163</td>
      <td>4542825</td>
    </tr>
    <tr>
      <th>409</th>
      <td>Tenkû no shiro Rapyuta</td>
      <td>1986</td>
      <td>U</td>
      <td>125</td>
      <td>Animation, Adventure, Drama</td>
      <td>8.0</td>
      <td>A young boy and a girl with a magic crystal mu...</td>
      <td>78.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Mayumi Tanaka</td>
      <td>Keiko Yokozawa</td>
      <td>Kotoe Hatsui</td>
      <td>Minori Terada</td>
      <td>150140</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>410</th>
      <td>The Terminator</td>
      <td>1984</td>
      <td>UA</td>
      <td>107</td>
      <td>Action, Sci-Fi</td>
      <td>8.0</td>
      <td>A human soldier is sent from 2029 to 1984 to s...</td>
      <td>84.00000</td>
      <td>James Cameron</td>
      <td>Arnold Schwarzenegger</td>
      <td>Linda Hamilton</td>
      <td>Michael Biehn</td>
      <td>Paul Winfield</td>
      <td>799795</td>
      <td>38400000</td>
    </tr>
    <tr>
      <th>411</th>
      <td>Gandhi</td>
      <td>1982</td>
      <td>U</td>
      <td>191</td>
      <td>Biography, Drama, History</td>
      <td>8.0</td>
      <td>The life of the lawyer who became the famed le...</td>
      <td>79.00000</td>
      <td>Richard Attenborough</td>
      <td>Ben Kingsley</td>
      <td>John Gielgud</td>
      <td>Rohini Hattangadi</td>
      <td>Roshan Seth</td>
      <td>217664</td>
      <td>52767889</td>
    </tr>
    <tr>
      <th>412</th>
      <td>Kagemusha</td>
      <td>1980</td>
      <td>U</td>
      <td>180</td>
      <td>Drama, History, War</td>
      <td>8.0</td>
      <td>A petty thief with an utter resemblance to a s...</td>
      <td>84.00000</td>
      <td>Akira Kurosawa</td>
      <td>Tatsuya Nakadai</td>
      <td>Tsutomu Yamazaki</td>
      <td>Ken'ichi Hagiwara</td>
      <td>Jinpachi Nezu</td>
      <td>32195</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>413</th>
      <td>Being There</td>
      <td>1979</td>
      <td>PG</td>
      <td>130</td>
      <td>Comedy, Drama</td>
      <td>8.0</td>
      <td>A simpleminded, sheltered gardener becomes an ...</td>
      <td>83.00000</td>
      <td>Hal Ashby</td>
      <td>Peter Sellers</td>
      <td>Shirley MacLaine</td>
      <td>Melvyn Douglas</td>
      <td>Jack Warden</td>
      <td>65625</td>
      <td>30177511</td>
    </tr>
    <tr>
      <th>414</th>
      <td>Annie Hall</td>
      <td>1977</td>
      <td>A</td>
      <td>93</td>
      <td>Comedy, Romance</td>
      <td>8.0</td>
      <td>Neurotic New York comedian Alvy Singer falls i...</td>
      <td>92.00000</td>
      <td>Woody Allen</td>
      <td>Woody Allen</td>
      <td>Diane Keaton</td>
      <td>Tony Roberts</td>
      <td>Carol Kane</td>
      <td>251823</td>
      <td>39200000</td>
    </tr>
    <tr>
      <th>415</th>
      <td>Jaws</td>
      <td>1975</td>
      <td>A</td>
      <td>124</td>
      <td>Adventure, Thriller</td>
      <td>8.0</td>
      <td>When a killer shark unleashes chaos on a beach...</td>
      <td>87.00000</td>
      <td>Steven Spielberg</td>
      <td>Roy Scheider</td>
      <td>Robert Shaw</td>
      <td>Richard Dreyfuss</td>
      <td>Lorraine Gary</td>
      <td>543388</td>
      <td>260000000</td>
    </tr>
    <tr>
      <th>416</th>
      <td>Dog Day Afternoon</td>
      <td>1975</td>
      <td>U</td>
      <td>125</td>
      <td>Biography, Crime, Drama</td>
      <td>8.0</td>
      <td>Three amateur bank robbers plan to hold up a b...</td>
      <td>86.00000</td>
      <td>Sidney Lumet</td>
      <td>Al Pacino</td>
      <td>John Cazale</td>
      <td>Penelope Allen</td>
      <td>Sully Boyar</td>
      <td>235652</td>
      <td>50000000</td>
    </tr>
    <tr>
      <th>417</th>
      <td>Young Frankenstein</td>
      <td>1974</td>
      <td>A</td>
      <td>106</td>
      <td>Comedy</td>
      <td>8.0</td>
      <td>An American grandson of the infamous scientist...</td>
      <td>80.00000</td>
      <td>Mel Brooks</td>
      <td>Gene Wilder</td>
      <td>Madeline Kahn</td>
      <td>Marty Feldman</td>
      <td>Peter Boyle</td>
      <td>143359</td>
      <td>86300000</td>
    </tr>
    <tr>
      <th>418</th>
      <td>Papillon</td>
      <td>1973</td>
      <td>R</td>
      <td>151</td>
      <td>Biography, Crime, Drama</td>
      <td>8.0</td>
      <td>A man befriends a fellow criminal as the two o...</td>
      <td>58.00000</td>
      <td>Franklin J. Schaffner</td>
      <td>Steve McQueen</td>
      <td>Dustin Hoffman</td>
      <td>Victor Jory</td>
      <td>Don Gordon</td>
      <td>121627</td>
      <td>53267000</td>
    </tr>
    <tr>
      <th>419</th>
      <td>The Exorcist</td>
      <td>1973</td>
      <td>A</td>
      <td>122</td>
      <td>Horror</td>
      <td>8.0</td>
      <td>When a 12-year-old girl is possessed by a myst...</td>
      <td>81.00000</td>
      <td>William Friedkin</td>
      <td>Ellen Burstyn</td>
      <td>Max von Sydow</td>
      <td>Linda Blair</td>
      <td>Lee J. Cobb</td>
      <td>362393</td>
      <td>232906145</td>
    </tr>
    <tr>
      <th>420</th>
      <td>Sleuth</td>
      <td>1972</td>
      <td>PG</td>
      <td>138</td>
      <td>Mystery, Thriller</td>
      <td>8.0</td>
      <td>A man who loves games and theater invites his ...</td>
      <td>77.97153</td>
      <td>Joseph L. Mankiewicz</td>
      <td>Laurence Olivier</td>
      <td>Michael Caine</td>
      <td>Alec Cawthorne</td>
      <td>John Matthews</td>
      <td>44748</td>
      <td>4081254</td>
    </tr>
    <tr>
      <th>421</th>
      <td>The Last Picture Show</td>
      <td>1971</td>
      <td>R</td>
      <td>118</td>
      <td>Drama, Romance</td>
      <td>8.0</td>
      <td>In 1951, a group of high schoolers come of age...</td>
      <td>93.00000</td>
      <td>Peter Bogdanovich</td>
      <td>Timothy Bottoms</td>
      <td>Jeff Bridges</td>
      <td>Cybill Shepherd</td>
      <td>Ben Johnson</td>
      <td>42456</td>
      <td>29133000</td>
    </tr>
    <tr>
      <th>422</th>
      <td>Fiddler on the Roof</td>
      <td>1971</td>
      <td>G</td>
      <td>181</td>
      <td>Drama, Family, Musical</td>
      <td>8.0</td>
      <td>In prerevolutionary Russia, a Jewish peasant c...</td>
      <td>67.00000</td>
      <td>Norman Jewison</td>
      <td>Topol</td>
      <td>Norma Crane</td>
      <td>Leonard Frey</td>
      <td>Molly Picon</td>
      <td>39491</td>
      <td>80500000</td>
    </tr>
    <tr>
      <th>423</th>
      <td>Il conformista</td>
      <td>1970</td>
      <td>UA</td>
      <td>113</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>A weak-willed Italian man becomes a fascist fl...</td>
      <td>100.00000</td>
      <td>Bernardo Bertolucci</td>
      <td>Jean-Louis Trintignant</td>
      <td>Stefania Sandrelli</td>
      <td>Gastone Moschin</td>
      <td>Enzo Tarascio</td>
      <td>27067</td>
      <td>541940</td>
    </tr>
    <tr>
      <th>424</th>
      <td>Butch Cassidy and the Sundance Kid</td>
      <td>1969</td>
      <td>PG</td>
      <td>110</td>
      <td>Biography, Crime, Drama</td>
      <td>8.0</td>
      <td>Wyoming, early 1900s. Butch Cassidy and The Su...</td>
      <td>66.00000</td>
      <td>George Roy Hill</td>
      <td>Paul Newman</td>
      <td>Robert Redford</td>
      <td>Katharine Ross</td>
      <td>Strother Martin</td>
      <td>201888</td>
      <td>102308889</td>
    </tr>
    <tr>
      <th>425</th>
      <td>Rosemary's Baby</td>
      <td>1968</td>
      <td>A</td>
      <td>137</td>
      <td>Drama, Horror</td>
      <td>8.0</td>
      <td>A young couple trying for a baby move into a f...</td>
      <td>96.00000</td>
      <td>Roman Polanski</td>
      <td>Mia Farrow</td>
      <td>John Cassavetes</td>
      <td>Ruth Gordon</td>
      <td>Sidney Blackmer</td>
      <td>193674</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>426</th>
      <td>Planet of the Apes</td>
      <td>1968</td>
      <td>U</td>
      <td>112</td>
      <td>Adventure, Sci-Fi</td>
      <td>8.0</td>
      <td>An astronaut crew crash-lands on a planet in t...</td>
      <td>79.00000</td>
      <td>Franklin J. Schaffner</td>
      <td>Charlton Heston</td>
      <td>Roddy McDowall</td>
      <td>Kim Hunter</td>
      <td>Maurice Evans</td>
      <td>165167</td>
      <td>33395426</td>
    </tr>
    <tr>
      <th>427</th>
      <td>The Graduate</td>
      <td>1967</td>
      <td>A</td>
      <td>106</td>
      <td>Comedy, Drama, Romance</td>
      <td>8.0</td>
      <td>A disillusioned college graduate finds himself...</td>
      <td>83.00000</td>
      <td>Mike Nichols</td>
      <td>Dustin Hoffman</td>
      <td>Anne Bancroft</td>
      <td>Katharine Ross</td>
      <td>William Daniels</td>
      <td>253676</td>
      <td>104945305</td>
    </tr>
    <tr>
      <th>428</th>
      <td>Who's Afraid of Virginia Woolf?</td>
      <td>1966</td>
      <td>A</td>
      <td>131</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>A bitter, aging couple, with the help of alcoh...</td>
      <td>75.00000</td>
      <td>Mike Nichols</td>
      <td>Elizabeth Taylor</td>
      <td>Richard Burton</td>
      <td>George Segal</td>
      <td>Sandy Dennis</td>
      <td>68926</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>429</th>
      <td>The Sound of Music</td>
      <td>1965</td>
      <td>U</td>
      <td>172</td>
      <td>Biography, Drama, Family</td>
      <td>8.0</td>
      <td>A woman leaves an Austrian convent to become a...</td>
      <td>63.00000</td>
      <td>Robert Wise</td>
      <td>Julie Andrews</td>
      <td>Christopher Plummer</td>
      <td>Eleanor Parker</td>
      <td>Richard Haydn</td>
      <td>205425</td>
      <td>163214286</td>
    </tr>
    <tr>
      <th>430</th>
      <td>Doctor Zhivago</td>
      <td>1965</td>
      <td>A</td>
      <td>197</td>
      <td>Drama, Romance, War</td>
      <td>8.0</td>
      <td>The life of a Russian physician and poet who, ...</td>
      <td>69.00000</td>
      <td>David Lean</td>
      <td>Omar Sharif</td>
      <td>Julie Christie</td>
      <td>Geraldine Chaplin</td>
      <td>Rod Steiger</td>
      <td>69903</td>
      <td>111722000</td>
    </tr>
    <tr>
      <th>431</th>
      <td>Per un pugno di dollari</td>
      <td>1964</td>
      <td>A</td>
      <td>99</td>
      <td>Action, Drama, Western</td>
      <td>8.0</td>
      <td>A wandering gunfighter plays two rival familie...</td>
      <td>65.00000</td>
      <td>Sergio Leone</td>
      <td>Clint Eastwood</td>
      <td>Gian Maria Volontè</td>
      <td>Marianne Koch</td>
      <td>Wolfgang Lukschy</td>
      <td>198219</td>
      <td>14500000</td>
    </tr>
    <tr>
      <th>432</th>
      <td>8½</td>
      <td>1963</td>
      <td>Unknown</td>
      <td>138</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>A harried movie director retreats into his mem...</td>
      <td>91.00000</td>
      <td>Federico Fellini</td>
      <td>Marcello Mastroianni</td>
      <td>Anouk Aimée</td>
      <td>Claudia Cardinale</td>
      <td>Sandra Milo</td>
      <td>108844</td>
      <td>50690</td>
    </tr>
    <tr>
      <th>433</th>
      <td>Vivre sa vie: Film en douze tableaux</td>
      <td>1962</td>
      <td>Unknown</td>
      <td>80</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>Twelve episodic tales in the life of a Parisia...</td>
      <td>77.97153</td>
      <td>Jean-Luc Godard</td>
      <td>Anna Karina</td>
      <td>Sady Rebbot</td>
      <td>André S. Labarthe</td>
      <td>Guylaine Schlumberger</td>
      <td>28057</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>434</th>
      <td>The Hustler</td>
      <td>1961</td>
      <td>A</td>
      <td>134</td>
      <td>Drama, Sport</td>
      <td>8.0</td>
      <td>An up-and-coming pool player plays a long-time...</td>
      <td>90.00000</td>
      <td>Robert Rossen</td>
      <td>Paul Newman</td>
      <td>Jackie Gleason</td>
      <td>Piper Laurie</td>
      <td>George C. Scott</td>
      <td>75067</td>
      <td>8284000</td>
    </tr>
    <tr>
      <th>435</th>
      <td>La dolce vita</td>
      <td>1960</td>
      <td>A</td>
      <td>174</td>
      <td>Comedy, Drama</td>
      <td>8.0</td>
      <td>A series of stories following a week in the li...</td>
      <td>95.00000</td>
      <td>Federico Fellini</td>
      <td>Marcello Mastroianni</td>
      <td>Anita Ekberg</td>
      <td>Anouk Aimée</td>
      <td>Yvonne Furneaux</td>
      <td>66621</td>
      <td>19516000</td>
    </tr>
    <tr>
      <th>436</th>
      <td>Rio Bravo</td>
      <td>1959</td>
      <td>Passed</td>
      <td>141</td>
      <td>Action, Drama, Western</td>
      <td>8.0</td>
      <td>A small-town sheriff in the American West enli...</td>
      <td>93.00000</td>
      <td>Howard Hawks</td>
      <td>John Wayne</td>
      <td>Dean Martin</td>
      <td>Ricky Nelson</td>
      <td>Angie Dickinson</td>
      <td>56305</td>
      <td>12535000</td>
    </tr>
    <tr>
      <th>437</th>
      <td>Anatomy of a Murder</td>
      <td>1959</td>
      <td>Unknown</td>
      <td>161</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.0</td>
      <td>In a murder trial, the defendant says he suffe...</td>
      <td>95.00000</td>
      <td>Otto Preminger</td>
      <td>James Stewart</td>
      <td>Lee Remick</td>
      <td>Ben Gazzara</td>
      <td>Arthur O'Connell</td>
      <td>59847</td>
      <td>11900000</td>
    </tr>
    <tr>
      <th>438</th>
      <td>Touch of Evil</td>
      <td>1958</td>
      <td>PG-13</td>
      <td>95</td>
      <td>Crime, Drama, Film-Noir</td>
      <td>8.0</td>
      <td>A stark, perverse story of murder, kidnapping,...</td>
      <td>99.00000</td>
      <td>Orson Welles</td>
      <td>Charlton Heston</td>
      <td>Orson Welles</td>
      <td>Janet Leigh</td>
      <td>Joseph Calleia</td>
      <td>98431</td>
      <td>2237659</td>
    </tr>
    <tr>
      <th>439</th>
      <td>Cat on a Hot Tin Roof</td>
      <td>1958</td>
      <td>A</td>
      <td>108</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>Brick is an alcoholic ex-football player who d...</td>
      <td>84.00000</td>
      <td>Richard Brooks</td>
      <td>Elizabeth Taylor</td>
      <td>Paul Newman</td>
      <td>Burl Ives</td>
      <td>Jack Carson</td>
      <td>45062</td>
      <td>17570324</td>
    </tr>
    <tr>
      <th>440</th>
      <td>Sweet Smell of Success</td>
      <td>1957</td>
      <td>Approved</td>
      <td>96</td>
      <td>Drama, Film-Noir</td>
      <td>8.0</td>
      <td>Powerful but unethical Broadway columnist J.J....</td>
      <td>100.00000</td>
      <td>Alexander Mackendrick</td>
      <td>Burt Lancaster</td>
      <td>Tony Curtis</td>
      <td>Susan Harrison</td>
      <td>Martin Milner</td>
      <td>28137</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>441</th>
      <td>The Killing</td>
      <td>1956</td>
      <td>Approved</td>
      <td>84</td>
      <td>Crime, Drama, Film-Noir</td>
      <td>8.0</td>
      <td>Crook Johnny Clay assembles a five man team to...</td>
      <td>91.00000</td>
      <td>Stanley Kubrick</td>
      <td>Sterling Hayden</td>
      <td>Coleen Gray</td>
      <td>Vince Edwards</td>
      <td>Jay C. Flippen</td>
      <td>81702</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>442</th>
      <td>The Night of the Hunter</td>
      <td>1955</td>
      <td>Unknown</td>
      <td>92</td>
      <td>Crime, Drama, Film-Noir</td>
      <td>8.0</td>
      <td>A religious fanatic marries a gullible widow w...</td>
      <td>99.00000</td>
      <td>Charles Laughton</td>
      <td>Robert Mitchum</td>
      <td>Shelley Winters</td>
      <td>Lillian Gish</td>
      <td>James Gleason</td>
      <td>81980</td>
      <td>654000</td>
    </tr>
    <tr>
      <th>443</th>
      <td>La Strada</td>
      <td>1954</td>
      <td>Unknown</td>
      <td>108</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>A care-free girl is sold to a traveling entert...</td>
      <td>77.97153</td>
      <td>Federico Fellini</td>
      <td>Anthony Quinn</td>
      <td>Giulietta Masina</td>
      <td>Richard Basehart</td>
      <td>Aldo Silvani</td>
      <td>58314</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>444</th>
      <td>Les diaboliques</td>
      <td>1955</td>
      <td>Unknown</td>
      <td>117</td>
      <td>Crime, Drama, Horror</td>
      <td>8.0</td>
      <td>The wife and mistress of a loathed school prin...</td>
      <td>77.97153</td>
      <td>Henri-Georges Clouzot</td>
      <td>Simone Signoret</td>
      <td>Véra Clouzot</td>
      <td>Paul Meurisse</td>
      <td>Charles Vanel</td>
      <td>61503</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>445</th>
      <td>Stalag 17</td>
      <td>1953</td>
      <td>Unknown</td>
      <td>120</td>
      <td>Comedy, Drama, War</td>
      <td>8.0</td>
      <td>When two escaping American World War II prison...</td>
      <td>84.00000</td>
      <td>Billy Wilder</td>
      <td>William Holden</td>
      <td>Don Taylor</td>
      <td>Otto Preminger</td>
      <td>Robert Strauss</td>
      <td>51046</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>446</th>
      <td>Roman Holiday</td>
      <td>1953</td>
      <td>Unknown</td>
      <td>118</td>
      <td>Comedy, Romance</td>
      <td>8.0</td>
      <td>A bored and sheltered princess escapes her gua...</td>
      <td>78.00000</td>
      <td>William Wyler</td>
      <td>Gregory Peck</td>
      <td>Audrey Hepburn</td>
      <td>Eddie Albert</td>
      <td>Hartley Power</td>
      <td>127256</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>447</th>
      <td>A Streetcar Named Desire</td>
      <td>1951</td>
      <td>A</td>
      <td>122</td>
      <td>Drama</td>
      <td>8.0</td>
      <td>Disturbed Blanche DuBois moves in with her sis...</td>
      <td>97.00000</td>
      <td>Elia Kazan</td>
      <td>Vivien Leigh</td>
      <td>Marlon Brando</td>
      <td>Kim Hunter</td>
      <td>Karl Malden</td>
      <td>99182</td>
      <td>8000000</td>
    </tr>
    <tr>
      <th>448</th>
      <td>In a Lonely Place</td>
      <td>1950</td>
      <td>Unknown</td>
      <td>94</td>
      <td>Drama, Film-Noir, Mystery</td>
      <td>8.0</td>
      <td>A potentially violent screenwriter is a murder...</td>
      <td>77.97153</td>
      <td>Nicholas Ray</td>
      <td>Humphrey Bogart</td>
      <td>Gloria Grahame</td>
      <td>Frank Lovejoy</td>
      <td>Carl Benton Reid</td>
      <td>26784</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>449</th>
      <td>Kind Hearts and Coronets</td>
      <td>1949</td>
      <td>U</td>
      <td>106</td>
      <td>Comedy, Crime</td>
      <td>8.0</td>
      <td>A distant poor relative of the Duke D'Ascoyne ...</td>
      <td>77.97153</td>
      <td>Robert Hamer</td>
      <td>Dennis Price</td>
      <td>Alec Guinness</td>
      <td>Valerie Hobson</td>
      <td>Joan Greenwood</td>
      <td>34485</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>450</th>
      <td>Rope</td>
      <td>1948</td>
      <td>A</td>
      <td>80</td>
      <td>Crime, Drama, Mystery</td>
      <td>8.0</td>
      <td>Two men attempt to prove they committed the pe...</td>
      <td>73.00000</td>
      <td>Alfred Hitchcock</td>
      <td>James Stewart</td>
      <td>John Dall</td>
      <td>Farley Granger</td>
      <td>Dick Hogan</td>
      <td>129783</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>451</th>
      <td>Out of the Past</td>
      <td>1947</td>
      <td>Unknown</td>
      <td>97</td>
      <td>Crime, Drama, Film-Noir</td>
      <td>8.0</td>
      <td>A private eye escapes his past to run a gas st...</td>
      <td>77.97153</td>
      <td>Jacques Tourneur</td>
      <td>Robert Mitchum</td>
      <td>Jane Greer</td>
      <td>Kirk Douglas</td>
      <td>Rhonda Fleming</td>
      <td>32784</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>452</th>
      <td>Brief Encounter</td>
      <td>1945</td>
      <td>U</td>
      <td>86</td>
      <td>Drama, Romance</td>
      <td>8.0</td>
      <td>Meeting a stranger in a railway station, a wom...</td>
      <td>92.00000</td>
      <td>David Lean</td>
      <td>Celia Johnson</td>
      <td>Trevor Howard</td>
      <td>Stanley Holloway</td>
      <td>Joyce Carey</td>
      <td>35601</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>453</th>
      <td>Laura</td>
      <td>1944</td>
      <td>Passed</td>
      <td>88</td>
      <td>Drama, Film-Noir, Mystery</td>
      <td>8.0</td>
      <td>A police detective falls in love with the woma...</td>
      <td>77.97153</td>
      <td>Otto Preminger</td>
      <td>Gene Tierney</td>
      <td>Dana Andrews</td>
      <td>Clifton Webb</td>
      <td>Vincent Price</td>
      <td>42725</td>
      <td>4360000</td>
    </tr>
    <tr>
      <th>454</th>
      <td>The Best Years of Our Lives</td>
      <td>1946</td>
      <td>Approved</td>
      <td>170</td>
      <td>Drama, Romance, War</td>
      <td>8.0</td>
      <td>Three World War II veterans return home to sma...</td>
      <td>93.00000</td>
      <td>William Wyler</td>
      <td>Myrna Loy</td>
      <td>Dana Andrews</td>
      <td>Fredric March</td>
      <td>Teresa Wright</td>
      <td>57259</td>
      <td>23650000</td>
    </tr>
    <tr>
      <th>455</th>
      <td>Arsenic and Old Lace</td>
      <td>1942</td>
      <td>Unknown</td>
      <td>118</td>
      <td>Comedy, Crime, Thriller</td>
      <td>8.0</td>
      <td>A writer of books on the futility of marriage ...</td>
      <td>77.97153</td>
      <td>Frank Capra</td>
      <td>Cary Grant</td>
      <td>Priscilla Lane</td>
      <td>Raymond Massey</td>
      <td>Jack Carson</td>
      <td>65101</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>456</th>
      <td>The Maltese Falcon</td>
      <td>1941</td>
      <td>Unknown</td>
      <td>100</td>
      <td>Film-Noir, Mystery</td>
      <td>8.0</td>
      <td>A private detective takes on a case that invol...</td>
      <td>96.00000</td>
      <td>John Huston</td>
      <td>Humphrey Bogart</td>
      <td>Mary Astor</td>
      <td>Gladys George</td>
      <td>Peter Lorre</td>
      <td>148928</td>
      <td>2108060</td>
    </tr>
    <tr>
      <th>457</th>
      <td>The Grapes of Wrath</td>
      <td>1940</td>
      <td>Passed</td>
      <td>129</td>
      <td>Drama, History</td>
      <td>8.0</td>
      <td>A poor Midwest family is forced off their land...</td>
      <td>96.00000</td>
      <td>John Ford</td>
      <td>Henry Fonda</td>
      <td>Jane Darwell</td>
      <td>John Carradine</td>
      <td>Charley Grapewin</td>
      <td>85559</td>
      <td>55000</td>
    </tr>
    <tr>
      <th>458</th>
      <td>The Wizard of Oz</td>
      <td>1939</td>
      <td>U</td>
      <td>102</td>
      <td>Adventure, Family, Fantasy</td>
      <td>8.0</td>
      <td>Dorothy Gale is swept away from a farm in Kans...</td>
      <td>92.00000</td>
      <td>Victor Fleming</td>
      <td>George Cukor</td>
      <td>Mervyn LeRoy</td>
      <td>Norman Taurog</td>
      <td>Richard Thorpe</td>
      <td>371379</td>
      <td>2076020</td>
    </tr>
    <tr>
      <th>459</th>
      <td>La règle du jeu</td>
      <td>1939</td>
      <td>Unknown</td>
      <td>110</td>
      <td>Comedy, Drama</td>
      <td>8.0</td>
      <td>A bourgeois life in France at the onset of Wor...</td>
      <td>77.97153</td>
      <td>Jean Renoir</td>
      <td>Marcel Dalio</td>
      <td>Nora Gregor</td>
      <td>Paulette Dubost</td>
      <td>Mila Parély</td>
      <td>26725</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>460</th>
      <td>The Thin Man</td>
      <td>1934</td>
      <td>TV-PG</td>
      <td>91</td>
      <td>Comedy, Crime, Mystery</td>
      <td>8.0</td>
      <td>Former detective Nick Charles and his wealthy ...</td>
      <td>86.00000</td>
      <td>W.S. Van Dyke</td>
      <td>William Powell</td>
      <td>Myrna Loy</td>
      <td>Maureen O'Sullivan</td>
      <td>Nat Pendleton</td>
      <td>26642</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>461</th>
      <td>All Quiet on the Western Front</td>
      <td>1930</td>
      <td>U</td>
      <td>152</td>
      <td>Drama, War</td>
      <td>8.0</td>
      <td>A German youth eagerly enters World War I, but...</td>
      <td>91.00000</td>
      <td>Lewis Milestone</td>
      <td>Lew Ayres</td>
      <td>Louis Wolheim</td>
      <td>John Wray</td>
      <td>Arnold Lucy</td>
      <td>57318</td>
      <td>3270000</td>
    </tr>
    <tr>
      <th>462</th>
      <td>Bronenosets Potemkin</td>
      <td>1925</td>
      <td>Unknown</td>
      <td>75</td>
      <td>Drama, History, Thriller</td>
      <td>8.0</td>
      <td>In the midst of the Russian Revolution of 1905...</td>
      <td>97.00000</td>
      <td>Sergei M. Eisenstein</td>
      <td>Aleksandr Antonov</td>
      <td>Vladimir Barskiy</td>
      <td>Grigoriy Aleksandrov</td>
      <td>Ivan Bobrov</td>
      <td>53054</td>
      <td>50970</td>
    </tr>
    <tr>
      <th>463</th>
      <td>Knives Out</td>
      <td>2019</td>
      <td>UA</td>
      <td>130</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.9</td>
      <td>A detective investigates the death of a patria...</td>
      <td>82.00000</td>
      <td>Rian Johnson</td>
      <td>Daniel Craig</td>
      <td>Chris Evans</td>
      <td>Ana de Armas</td>
      <td>Jamie Lee Curtis</td>
      <td>454203</td>
      <td>165359751</td>
    </tr>
    <tr>
      <th>464</th>
      <td>Dil Bechara</td>
      <td>2020</td>
      <td>UA</td>
      <td>101</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.9</td>
      <td>The emotional journey of two hopelessly in lov...</td>
      <td>77.97153</td>
      <td>Mukesh Chhabra</td>
      <td>Sushant Singh Rajput</td>
      <td>Sanjana Sanghi</td>
      <td>Sahil Vaid</td>
      <td>Saswata Chatterjee</td>
      <td>111478</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>465</th>
      <td>Manbiki kazoku</td>
      <td>2018</td>
      <td>A</td>
      <td>121</td>
      <td>Crime, Drama</td>
      <td>7.9</td>
      <td>A family of small-time crooks take in a child ...</td>
      <td>93.00000</td>
      <td>Hirokazu Koreeda</td>
      <td>Lily Franky</td>
      <td>Sakura Andô</td>
      <td>Kirin Kiki</td>
      <td>Mayu Matsuoka</td>
      <td>62754</td>
      <td>3313513</td>
    </tr>
    <tr>
      <th>466</th>
      <td>Marriage Story</td>
      <td>2019</td>
      <td>U</td>
      <td>137</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.9</td>
      <td>Noah Baumbach's incisive and compassionate loo...</td>
      <td>94.00000</td>
      <td>Noah Baumbach</td>
      <td>Adam Driver</td>
      <td>Scarlett Johansson</td>
      <td>Julia Greer</td>
      <td>Azhy Robertson</td>
      <td>246644</td>
      <td>2000000</td>
    </tr>
    <tr>
      <th>467</th>
      <td>Call Me by Your Name</td>
      <td>2017</td>
      <td>UA</td>
      <td>132</td>
      <td>Drama, Romance</td>
      <td>7.9</td>
      <td>In 1980s Italy, romance blossoms between a sev...</td>
      <td>93.00000</td>
      <td>Luca Guadagnino</td>
      <td>Armie Hammer</td>
      <td>Timothée Chalamet</td>
      <td>Michael Stuhlbarg</td>
      <td>Amira Casar</td>
      <td>212651</td>
      <td>18095701</td>
    </tr>
    <tr>
      <th>468</th>
      <td>I, Daniel Blake</td>
      <td>2016</td>
      <td>UA</td>
      <td>100</td>
      <td>Drama</td>
      <td>7.9</td>
      <td>After having suffered a heart-attack, a 59-yea...</td>
      <td>78.00000</td>
      <td>Ken Loach</td>
      <td>Laura Obiols</td>
      <td>Dave Johns</td>
      <td>Hayley Squires</td>
      <td>Sharon Percy</td>
      <td>53818</td>
      <td>258168</td>
    </tr>
    <tr>
      <th>469</th>
      <td>Isle of Dogs</td>
      <td>2018</td>
      <td>U</td>
      <td>101</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.9</td>
      <td>Set in Japan, Isle of Dogs follows a boy's ody...</td>
      <td>82.00000</td>
      <td>Wes Anderson</td>
      <td>Bryan Cranston</td>
      <td>Koyu Rankin</td>
      <td>Edward Norton</td>
      <td>Bob Balaban</td>
      <td>139114</td>
      <td>32015231</td>
    </tr>
    <tr>
      <th>470</th>
      <td>Hunt for the Wilderpeople</td>
      <td>2016</td>
      <td>UA</td>
      <td>101</td>
      <td>Adventure, Comedy, Drama</td>
      <td>7.9</td>
      <td>A national manhunt is ordered for a rebellious...</td>
      <td>81.00000</td>
      <td>Taika Waititi</td>
      <td>Sam Neill</td>
      <td>Julian Dennison</td>
      <td>Rima Te Wiata</td>
      <td>Rachel House</td>
      <td>111483</td>
      <td>5202582</td>
    </tr>
    <tr>
      <th>471</th>
      <td>Captain Fantastic</td>
      <td>2016</td>
      <td>R</td>
      <td>118</td>
      <td>Comedy, Drama</td>
      <td>7.9</td>
      <td>In the forests of the Pacific Northwest, a fat...</td>
      <td>72.00000</td>
      <td>Matt Ross</td>
      <td>Viggo Mortensen</td>
      <td>George MacKay</td>
      <td>Samantha Isler</td>
      <td>Annalise Basso</td>
      <td>189400</td>
      <td>5875006</td>
    </tr>
    <tr>
      <th>472</th>
      <td>Sing Street</td>
      <td>2016</td>
      <td>PG-13</td>
      <td>106</td>
      <td>Comedy, Drama, Music</td>
      <td>7.9</td>
      <td>A boy growing up in Dublin during the 1980s es...</td>
      <td>79.00000</td>
      <td>John Carney</td>
      <td>Ferdia Walsh-Peelo</td>
      <td>Aidan Gillen</td>
      <td>Maria Doyle Kennedy</td>
      <td>Jack Reynor</td>
      <td>85109</td>
      <td>3237118</td>
    </tr>
    <tr>
      <th>473</th>
      <td>Thor: Ragnarok</td>
      <td>2017</td>
      <td>UA</td>
      <td>130</td>
      <td>Action, Adventure, Comedy</td>
      <td>7.9</td>
      <td>Imprisoned on the planet Sakaar, Thor must rac...</td>
      <td>74.00000</td>
      <td>Taika Waititi</td>
      <td>Chris Hemsworth</td>
      <td>Tom Hiddleston</td>
      <td>Cate Blanchett</td>
      <td>Mark Ruffalo</td>
      <td>587775</td>
      <td>315058289</td>
    </tr>
    <tr>
      <th>474</th>
      <td>Nightcrawler</td>
      <td>2014</td>
      <td>A</td>
      <td>117</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.9</td>
      <td>When Louis Bloom, a con man desperate for work...</td>
      <td>76.00000</td>
      <td>Dan Gilroy</td>
      <td>Jake Gyllenhaal</td>
      <td>Rene Russo</td>
      <td>Bill Paxton</td>
      <td>Riz Ahmed</td>
      <td>466134</td>
      <td>32381218</td>
    </tr>
    <tr>
      <th>475</th>
      <td>Jojo Rabbit</td>
      <td>2019</td>
      <td>UA</td>
      <td>108</td>
      <td>Comedy, Drama, War</td>
      <td>7.9</td>
      <td>A young boy in Hitler's army finds out his mot...</td>
      <td>58.00000</td>
      <td>Taika Waititi</td>
      <td>Roman Griffin Davis</td>
      <td>Thomasin McKenzie</td>
      <td>Scarlett Johansson</td>
      <td>Taika Waititi</td>
      <td>297918</td>
      <td>349555</td>
    </tr>
    <tr>
      <th>476</th>
      <td>Arrival</td>
      <td>2016</td>
      <td>UA</td>
      <td>116</td>
      <td>Drama, Sci-Fi</td>
      <td>7.9</td>
      <td>A linguist works with the military to communic...</td>
      <td>81.00000</td>
      <td>Denis Villeneuve</td>
      <td>Amy Adams</td>
      <td>Jeremy Renner</td>
      <td>Forest Whitaker</td>
      <td>Michael Stuhlbarg</td>
      <td>594181</td>
      <td>100546139</td>
    </tr>
    <tr>
      <th>477</th>
      <td>Star Wars: Episode VII - The Force Awakens</td>
      <td>2015</td>
      <td>U</td>
      <td>138</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.9</td>
      <td>As a new threat to the galaxy rises, Rey, a de...</td>
      <td>80.00000</td>
      <td>J.J. Abrams</td>
      <td>Daisy Ridley</td>
      <td>John Boyega</td>
      <td>Oscar Isaac</td>
      <td>Domhnall Gleeson</td>
      <td>860823</td>
      <td>936662225</td>
    </tr>
    <tr>
      <th>478</th>
      <td>Before Midnight</td>
      <td>2013</td>
      <td>R</td>
      <td>109</td>
      <td>Drama, Romance</td>
      <td>7.9</td>
      <td>We meet Jesse and Celine nine years on in Gree...</td>
      <td>94.00000</td>
      <td>Richard Linklater</td>
      <td>Ethan Hawke</td>
      <td>Julie Delpy</td>
      <td>Seamus Davey-Fitzpatrick</td>
      <td>Ariane Labed</td>
      <td>141457</td>
      <td>8114627</td>
    </tr>
    <tr>
      <th>479</th>
      <td>X-Men: Days of Future Past</td>
      <td>2014</td>
      <td>UA</td>
      <td>132</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.9</td>
      <td>The X-Men send Wolverine to the past in a desp...</td>
      <td>75.00000</td>
      <td>Bryan Singer</td>
      <td>Patrick Stewart</td>
      <td>Ian McKellen</td>
      <td>Hugh Jackman</td>
      <td>James McAvoy</td>
      <td>659763</td>
      <td>233921534</td>
    </tr>
    <tr>
      <th>480</th>
      <td>Bir Zamanlar Anadolu'da</td>
      <td>2011</td>
      <td>Unknown</td>
      <td>157</td>
      <td>Crime, Drama</td>
      <td>7.9</td>
      <td>A group of men set out in search of a dead bod...</td>
      <td>82.00000</td>
      <td>Nuri Bilge Ceylan</td>
      <td>Muhammet Uzuner</td>
      <td>Yilmaz Erdogan</td>
      <td>Taner Birsel</td>
      <td>Ahmet Mümtaz Taylan</td>
      <td>41995</td>
      <td>138730</td>
    </tr>
    <tr>
      <th>481</th>
      <td>The Artist</td>
      <td>2011</td>
      <td>U</td>
      <td>100</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.9</td>
      <td>An egomaniacal film star develops a relationsh...</td>
      <td>89.00000</td>
      <td>Michel Hazanavicius</td>
      <td>Jean Dujardin</td>
      <td>Bérénice Bejo</td>
      <td>John Goodman</td>
      <td>James Cromwell</td>
      <td>230624</td>
      <td>44671682</td>
    </tr>
    <tr>
      <th>482</th>
      <td>Edge of Tomorrow</td>
      <td>2014</td>
      <td>UA</td>
      <td>113</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.9</td>
      <td>A soldier fighting aliens gets to relive the s...</td>
      <td>71.00000</td>
      <td>Doug Liman</td>
      <td>Tom Cruise</td>
      <td>Emily Blunt</td>
      <td>Bill Paxton</td>
      <td>Brendan Gleeson</td>
      <td>600004</td>
      <td>100206256</td>
    </tr>
    <tr>
      <th>483</th>
      <td>Amour</td>
      <td>2012</td>
      <td>UA</td>
      <td>127</td>
      <td>Drama, Romance</td>
      <td>7.9</td>
      <td>Georges and Anne are an octogenarian couple. T...</td>
      <td>94.00000</td>
      <td>Michael Haneke</td>
      <td>Jean-Louis Trintignant</td>
      <td>Emmanuelle Riva</td>
      <td>Isabelle Huppert</td>
      <td>Alexandre Tharaud</td>
      <td>93090</td>
      <td>6739492</td>
    </tr>
    <tr>
      <th>484</th>
      <td>The Irishman</td>
      <td>2019</td>
      <td>R</td>
      <td>209</td>
      <td>Biography, Crime, Drama</td>
      <td>7.9</td>
      <td>An old man recalls his time painting houses fo...</td>
      <td>94.00000</td>
      <td>Martin Scorsese</td>
      <td>Robert De Niro</td>
      <td>Al Pacino</td>
      <td>Joe Pesci</td>
      <td>Harvey Keitel</td>
      <td>324720</td>
      <td>7000000</td>
    </tr>
    <tr>
      <th>485</th>
      <td>Un prophète</td>
      <td>2009</td>
      <td>A</td>
      <td>155</td>
      <td>Crime, Drama</td>
      <td>7.9</td>
      <td>A young Arab man is sent to a French prison.</td>
      <td>90.00000</td>
      <td>Jacques Audiard</td>
      <td>Tahar Rahim</td>
      <td>Niels Arestrup</td>
      <td>Adel Bencherif</td>
      <td>Reda Kateb</td>
      <td>93560</td>
      <td>2084637</td>
    </tr>
    <tr>
      <th>486</th>
      <td>Moon</td>
      <td>2009</td>
      <td>R</td>
      <td>97</td>
      <td>Drama, Mystery, Sci-Fi</td>
      <td>7.9</td>
      <td>Astronaut Sam Bell has a quintessentially pers...</td>
      <td>67.00000</td>
      <td>Duncan Jones</td>
      <td>Sam Rockwell</td>
      <td>Kevin Spacey</td>
      <td>Dominique McElligott</td>
      <td>Rosie Shaw</td>
      <td>335152</td>
      <td>5009677</td>
    </tr>
    <tr>
      <th>487</th>
      <td>Låt den rätte komma in</td>
      <td>2008</td>
      <td>R</td>
      <td>114</td>
      <td>Crime, Drama, Fantasy</td>
      <td>7.9</td>
      <td>Oskar, an overlooked and bullied boy, finds lo...</td>
      <td>82.00000</td>
      <td>Tomas Alfredson</td>
      <td>Kåre Hedebrant</td>
      <td>Lina Leandersson</td>
      <td>Per Ragnar</td>
      <td>Henrik Dahl</td>
      <td>205609</td>
      <td>2122065</td>
    </tr>
    <tr>
      <th>488</th>
      <td>District 9</td>
      <td>2009</td>
      <td>A</td>
      <td>112</td>
      <td>Action, Sci-Fi, Thriller</td>
      <td>7.9</td>
      <td>Violence ensues after an extraterrestrial race...</td>
      <td>81.00000</td>
      <td>Neill Blomkamp</td>
      <td>Sharlto Copley</td>
      <td>David James</td>
      <td>Jason Cope</td>
      <td>Nathalie Boltt</td>
      <td>638202</td>
      <td>115646235</td>
    </tr>
    <tr>
      <th>489</th>
      <td>The Wrestler</td>
      <td>2008</td>
      <td>UA</td>
      <td>109</td>
      <td>Drama, Sport</td>
      <td>7.9</td>
      <td>A faded professional wrestler must retire, but...</td>
      <td>80.00000</td>
      <td>Darren Aronofsky</td>
      <td>Mickey Rourke</td>
      <td>Marisa Tomei</td>
      <td>Evan Rachel Wood</td>
      <td>Mark Margolis</td>
      <td>289415</td>
      <td>26236603</td>
    </tr>
    <tr>
      <th>490</th>
      <td>Jab We Met</td>
      <td>2007</td>
      <td>U</td>
      <td>138</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.9</td>
      <td>A depressed wealthy businessman finds his life...</td>
      <td>77.97153</td>
      <td>Imtiaz Ali</td>
      <td>Shahid Kapoor</td>
      <td>Kareena Kapoor</td>
      <td>Tarun Arora</td>
      <td>Dara Singh</td>
      <td>47720</td>
      <td>410800</td>
    </tr>
    <tr>
      <th>491</th>
      <td>Boyhood</td>
      <td>2014</td>
      <td>A</td>
      <td>165</td>
      <td>Drama</td>
      <td>7.9</td>
      <td>The life of Mason, from early childhood to his...</td>
      <td>100.00000</td>
      <td>Richard Linklater</td>
      <td>Ellar Coltrane</td>
      <td>Patricia Arquette</td>
      <td>Ethan Hawke</td>
      <td>Elijah Smith</td>
      <td>335533</td>
      <td>25379975</td>
    </tr>
    <tr>
      <th>492</th>
      <td>4 luni, 3 saptamâni si 2 zile</td>
      <td>2007</td>
      <td>Unknown</td>
      <td>113</td>
      <td>Drama</td>
      <td>7.9</td>
      <td>A woman assists her friend in arranging an ill...</td>
      <td>97.00000</td>
      <td>Cristian Mungiu</td>
      <td>Anamaria Marinca</td>
      <td>Laura Vasiliu</td>
      <td>Vlad Ivanov</td>
      <td>Alexandru Potocean</td>
      <td>56625</td>
      <td>1185783</td>
    </tr>
    <tr>
      <th>493</th>
      <td>Star Trek</td>
      <td>2009</td>
      <td>UA</td>
      <td>127</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.9</td>
      <td>The brash James T. Kirk tries to live up to hi...</td>
      <td>82.00000</td>
      <td>J.J. Abrams</td>
      <td>Chris Pine</td>
      <td>Zachary Quinto</td>
      <td>Simon Pegg</td>
      <td>Leonard Nimoy</td>
      <td>577336</td>
      <td>257730019</td>
    </tr>
    <tr>
      <th>494</th>
      <td>In Bruges</td>
      <td>2008</td>
      <td>R</td>
      <td>107</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.9</td>
      <td>Guilt-stricken after a job gone wrong, hitman ...</td>
      <td>67.00000</td>
      <td>Martin McDonagh</td>
      <td>Colin Farrell</td>
      <td>Brendan Gleeson</td>
      <td>Ciarán Hinds</td>
      <td>Elizabeth Berrington</td>
      <td>390334</td>
      <td>7757130</td>
    </tr>
    <tr>
      <th>495</th>
      <td>The Man from Earth</td>
      <td>2007</td>
      <td>Unknown</td>
      <td>87</td>
      <td>Drama, Fantasy, Mystery</td>
      <td>7.9</td>
      <td>An impromptu goodbye party for Professor John ...</td>
      <td>77.97153</td>
      <td>Richard Schenkman</td>
      <td>David Lee Smith</td>
      <td>Tony Todd</td>
      <td>John Billingsley</td>
      <td>Ellen Crawford</td>
      <td>174125</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>496</th>
      <td>Letters from Iwo Jima</td>
      <td>2006</td>
      <td>UA</td>
      <td>141</td>
      <td>Action, Adventure, Drama</td>
      <td>7.9</td>
      <td>The story of the battle of Iwo Jima between th...</td>
      <td>89.00000</td>
      <td>Clint Eastwood</td>
      <td>Ken Watanabe</td>
      <td>Kazunari Ninomiya</td>
      <td>Tsuyoshi Ihara</td>
      <td>Ryô Kase</td>
      <td>154011</td>
      <td>13756082</td>
    </tr>
    <tr>
      <th>497</th>
      <td>The Fall</td>
      <td>2006</td>
      <td>R</td>
      <td>117</td>
      <td>Adventure, Drama, Fantasy</td>
      <td>7.9</td>
      <td>In a hospital on the outskirts of 1920s Los An...</td>
      <td>64.00000</td>
      <td>Tarsem Singh</td>
      <td>Lee Pace</td>
      <td>Catinca Untaru</td>
      <td>Justine Waddell</td>
      <td>Kim Uylenbroek</td>
      <td>107290</td>
      <td>2280348</td>
    </tr>
    <tr>
      <th>498</th>
      <td>Life of Pi</td>
      <td>2012</td>
      <td>U</td>
      <td>127</td>
      <td>Adventure, Drama, Fantasy</td>
      <td>7.9</td>
      <td>A young man who survives a disaster at sea is ...</td>
      <td>79.00000</td>
      <td>Ang Lee</td>
      <td>Suraj Sharma</td>
      <td>Irrfan Khan</td>
      <td>Adil Hussain</td>
      <td>Tabu</td>
      <td>580708</td>
      <td>124987023</td>
    </tr>
    <tr>
      <th>499</th>
      <td>Fantastic Mr. Fox</td>
      <td>2009</td>
      <td>PG</td>
      <td>87</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.9</td>
      <td>An urbane fox cannot resist returning to his f...</td>
      <td>83.00000</td>
      <td>Wes Anderson</td>
      <td>George Clooney</td>
      <td>Meryl Streep</td>
      <td>Bill Murray</td>
      <td>Jason Schwartzman</td>
      <td>199696</td>
      <td>21002919</td>
    </tr>
    <tr>
      <th>500</th>
      <td>C.R.A.Z.Y.</td>
      <td>2005</td>
      <td>Unknown</td>
      <td>129</td>
      <td>Comedy, Drama</td>
      <td>7.9</td>
      <td>A young French-Canadian, growing up in the 196...</td>
      <td>81.00000</td>
      <td>Jean-Marc Vallée</td>
      <td>Michel Côté</td>
      <td>Marc-André Grondin</td>
      <td>Danielle Proulx</td>
      <td>Émile Vallée</td>
      <td>31476</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>501</th>
      <td>Les choristes</td>
      <td>2004</td>
      <td>PG-13</td>
      <td>97</td>
      <td>Drama, Music</td>
      <td>7.9</td>
      <td>The new teacher at a severely administered boy...</td>
      <td>56.00000</td>
      <td>Christophe Barratier</td>
      <td>Gérard Jugnot</td>
      <td>François Berléand</td>
      <td>Jean-Baptiste Maunier</td>
      <td>Kad Merad</td>
      <td>57430</td>
      <td>3635164</td>
    </tr>
    <tr>
      <th>502</th>
      <td>Iron Man</td>
      <td>2008</td>
      <td>UA</td>
      <td>126</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.9</td>
      <td>After being held captive in an Afghan cave, bi...</td>
      <td>79.00000</td>
      <td>Jon Favreau</td>
      <td>Robert Downey Jr.</td>
      <td>Gwyneth Paltrow</td>
      <td>Terrence Howard</td>
      <td>Jeff Bridges</td>
      <td>939644</td>
      <td>318412101</td>
    </tr>
    <tr>
      <th>503</th>
      <td>Shaun of the Dead</td>
      <td>2004</td>
      <td>UA</td>
      <td>99</td>
      <td>Comedy, Horror</td>
      <td>7.9</td>
      <td>A man's uneventful life is disrupted by the zo...</td>
      <td>76.00000</td>
      <td>Edgar Wright</td>
      <td>Simon Pegg</td>
      <td>Nick Frost</td>
      <td>Kate Ashfield</td>
      <td>Lucy Davis</td>
      <td>512249</td>
      <td>13542874</td>
    </tr>
    <tr>
      <th>504</th>
      <td>Gegen die Wand</td>
      <td>2004</td>
      <td>R</td>
      <td>121</td>
      <td>Drama, Romance</td>
      <td>7.9</td>
      <td>With the intention to break free from the stri...</td>
      <td>78.00000</td>
      <td>Fatih Akin</td>
      <td>Birol Ünel</td>
      <td>Sibel Kekilli</td>
      <td>Güven Kiraç</td>
      <td>Zarah Jane McKenzie</td>
      <td>51325</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>505</th>
      <td>Mystic River</td>
      <td>2003</td>
      <td>A</td>
      <td>138</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.9</td>
      <td>The lives of three men who were childhood frie...</td>
      <td>84.00000</td>
      <td>Clint Eastwood</td>
      <td>Sean Penn</td>
      <td>Tim Robbins</td>
      <td>Kevin Bacon</td>
      <td>Emmy Rossum</td>
      <td>419420</td>
      <td>90135191</td>
    </tr>
    <tr>
      <th>506</th>
      <td>Harry Potter and the Prisoner of Azkaban</td>
      <td>2004</td>
      <td>U</td>
      <td>142</td>
      <td>Adventure, Family, Fantasy</td>
      <td>7.9</td>
      <td>Harry Potter, Ron and Hermione return to Hogwa...</td>
      <td>82.00000</td>
      <td>Alfonso Cuarón</td>
      <td>Daniel Radcliffe</td>
      <td>Emma Watson</td>
      <td>Rupert Grint</td>
      <td>Richard Griffiths</td>
      <td>552493</td>
      <td>249358727</td>
    </tr>
    <tr>
      <th>507</th>
      <td>Ying xiong</td>
      <td>2002</td>
      <td>PG-13</td>
      <td>120</td>
      <td>Action, Adventure, History</td>
      <td>7.9</td>
      <td>A defense officer, Nameless, was summoned by t...</td>
      <td>85.00000</td>
      <td>Yimou Zhang</td>
      <td>Jet Li</td>
      <td>Tony Chiu-Wai Leung</td>
      <td>Maggie Cheung</td>
      <td>Ziyi Zhang</td>
      <td>173999</td>
      <td>53710019</td>
    </tr>
    <tr>
      <th>508</th>
      <td>Hable con ella</td>
      <td>2002</td>
      <td>R</td>
      <td>112</td>
      <td>Drama, Mystery, Romance</td>
      <td>7.9</td>
      <td>Two men share an odd friendship while they car...</td>
      <td>86.00000</td>
      <td>Pedro Almodóvar</td>
      <td>Rosario Flores</td>
      <td>Javier Cámara</td>
      <td>Darío Grandinetti</td>
      <td>Leonor Watling</td>
      <td>104691</td>
      <td>9284265</td>
    </tr>
    <tr>
      <th>509</th>
      <td>No Man's Land</td>
      <td>2001</td>
      <td>R</td>
      <td>98</td>
      <td>Comedy, Drama, War</td>
      <td>7.9</td>
      <td>Bosnia and Herzegovina during 1993 at the time...</td>
      <td>84.00000</td>
      <td>Danis Tanovic</td>
      <td>Branko Djuric</td>
      <td>Rene Bitorajac</td>
      <td>Filip Sovagovic</td>
      <td>Georges Siatidis</td>
      <td>44618</td>
      <td>1059830</td>
    </tr>
    <tr>
      <th>510</th>
      <td>Cowboy Bebop: Tengoku no tobira</td>
      <td>2001</td>
      <td>U</td>
      <td>115</td>
      <td>Animation, Action, Crime</td>
      <td>7.9</td>
      <td>A terrorist explosion releases a deadly virus ...</td>
      <td>61.00000</td>
      <td>Shin'ichirô Watanabe</td>
      <td>Tensai Okamura</td>
      <td>Hiroyuki Okiura</td>
      <td>Yoshiyuki Takei</td>
      <td>Beau Billingslea</td>
      <td>42897</td>
      <td>1000045</td>
    </tr>
    <tr>
      <th>511</th>
      <td>The Bourne Identity</td>
      <td>2002</td>
      <td>UA</td>
      <td>119</td>
      <td>Action, Mystery, Thriller</td>
      <td>7.9</td>
      <td>A man is picked up by a fishing boat, bullet-r...</td>
      <td>68.00000</td>
      <td>Doug Liman</td>
      <td>Franka Potente</td>
      <td>Matt Damon</td>
      <td>Chris Cooper</td>
      <td>Clive Owen</td>
      <td>508771</td>
      <td>121661683</td>
    </tr>
    <tr>
      <th>512</th>
      <td>Nueve reinas</td>
      <td>2000</td>
      <td>R</td>
      <td>114</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.9</td>
      <td>Two con artists try to swindle a stamp collect...</td>
      <td>80.00000</td>
      <td>Fabián Bielinsky</td>
      <td>Ricardo Darín</td>
      <td>Gastón Pauls</td>
      <td>Graciela Tenenbaum</td>
      <td>María Mercedes Villagra</td>
      <td>49721</td>
      <td>1221261</td>
    </tr>
    <tr>
      <th>513</th>
      <td>Children of Men</td>
      <td>2006</td>
      <td>A</td>
      <td>109</td>
      <td>Adventure, Drama, Sci-Fi</td>
      <td>7.9</td>
      <td>In 2027, in a chaotic world in which women hav...</td>
      <td>84.00000</td>
      <td>Alfonso Cuarón</td>
      <td>Julianne Moore</td>
      <td>Clive Owen</td>
      <td>Chiwetel Ejiofor</td>
      <td>Michael Caine</td>
      <td>465113</td>
      <td>35552383</td>
    </tr>
    <tr>
      <th>514</th>
      <td>Almost Famous</td>
      <td>2000</td>
      <td>A</td>
      <td>122</td>
      <td>Adventure, Comedy, Drama</td>
      <td>7.9</td>
      <td>A high-school boy is given the chance to write...</td>
      <td>90.00000</td>
      <td>Cameron Crowe</td>
      <td>Billy Crudup</td>
      <td>Patrick Fugit</td>
      <td>Kate Hudson</td>
      <td>Frances McDormand</td>
      <td>252586</td>
      <td>32534850</td>
    </tr>
    <tr>
      <th>515</th>
      <td>Mulholland Dr.</td>
      <td>2001</td>
      <td>R</td>
      <td>147</td>
      <td>Drama, Mystery, Thriller</td>
      <td>7.9</td>
      <td>After a car wreck on the winding Mulholland Dr...</td>
      <td>85.00000</td>
      <td>David Lynch</td>
      <td>Naomi Watts</td>
      <td>Laura Harring</td>
      <td>Justin Theroux</td>
      <td>Jeanne Bates</td>
      <td>322031</td>
      <td>7220243</td>
    </tr>
    <tr>
      <th>516</th>
      <td>Toy Story 2</td>
      <td>1999</td>
      <td>U</td>
      <td>92</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.9</td>
      <td>When Woody is stolen by a toy collector, Buzz ...</td>
      <td>88.00000</td>
      <td>John Lasseter</td>
      <td>Ash Brannon</td>
      <td>Lee Unkrich</td>
      <td>Tom Hanks</td>
      <td>Tim Allen</td>
      <td>527512</td>
      <td>245852179</td>
    </tr>
    <tr>
      <th>517</th>
      <td>Boogie Nights</td>
      <td>1997</td>
      <td>R</td>
      <td>155</td>
      <td>Drama</td>
      <td>7.9</td>
      <td>Back when sex was safe, pleasure was a busines...</td>
      <td>85.00000</td>
      <td>Paul Thomas Anderson</td>
      <td>Mark Wahlberg</td>
      <td>Julianne Moore</td>
      <td>Burt Reynolds</td>
      <td>Luis Guzmán</td>
      <td>239473</td>
      <td>26400640</td>
    </tr>
    <tr>
      <th>518</th>
      <td>Mimi wo sumaseba</td>
      <td>1995</td>
      <td>U</td>
      <td>111</td>
      <td>Animation, Drama, Family</td>
      <td>7.9</td>
      <td>A love story between a girl who loves reading ...</td>
      <td>75.00000</td>
      <td>Yoshifumi Kondô</td>
      <td>Yoko Honna</td>
      <td>Issey Takahashi</td>
      <td>Takashi Tachibana</td>
      <td>Shigeru Muroi</td>
      <td>51943</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>519</th>
      <td>Once Were Warriors</td>
      <td>1994</td>
      <td>A</td>
      <td>102</td>
      <td>Crime, Drama</td>
      <td>7.9</td>
      <td>A family descended from Maori warriors is bede...</td>
      <td>77.00000</td>
      <td>Lee Tamahori</td>
      <td>Rena Owen</td>
      <td>Temuera Morrison</td>
      <td>Mamaengaroa Kerr-Bell</td>
      <td>Julian Arahanga</td>
      <td>31590</td>
      <td>2201126</td>
    </tr>
    <tr>
      <th>520</th>
      <td>True Romance</td>
      <td>1993</td>
      <td>R</td>
      <td>119</td>
      <td>Crime, Drama, Romance</td>
      <td>7.9</td>
      <td>In Detroit, a lonely pop culture geek marries ...</td>
      <td>59.00000</td>
      <td>Tony Scott</td>
      <td>Christian Slater</td>
      <td>Patricia Arquette</td>
      <td>Dennis Hopper</td>
      <td>Val Kilmer</td>
      <td>206918</td>
      <td>12281500</td>
    </tr>
    <tr>
      <th>521</th>
      <td>Trois couleurs: Bleu</td>
      <td>1993</td>
      <td>U</td>
      <td>94</td>
      <td>Drama, Music, Mystery</td>
      <td>7.9</td>
      <td>A woman struggles to find a way to live her li...</td>
      <td>85.00000</td>
      <td>Krzysztof Kieslowski</td>
      <td>Juliette Binoche</td>
      <td>Zbigniew Zamachowski</td>
      <td>Julie Delpy</td>
      <td>Benoît Régent</td>
      <td>89836</td>
      <td>1324974</td>
    </tr>
    <tr>
      <th>522</th>
      <td>Jûbê ninpûchô</td>
      <td>1993</td>
      <td>A</td>
      <td>94</td>
      <td>Animation, Action, Adventure</td>
      <td>7.9</td>
      <td>A vagabond swordsman is aided by a beautiful n...</td>
      <td>77.97153</td>
      <td>Yoshiaki Kawajiri</td>
      <td>Kôichi Yamadera</td>
      <td>Emi Shinohara</td>
      <td>Takeshi Aono</td>
      <td>Osamu Saka</td>
      <td>34529</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>523</th>
      <td>Carlito's Way</td>
      <td>1993</td>
      <td>A</td>
      <td>144</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.9</td>
      <td>A Puerto Rican former convict, just released f...</td>
      <td>65.00000</td>
      <td>Brian De Palma</td>
      <td>Al Pacino</td>
      <td>Sean Penn</td>
      <td>Penelope Ann Miller</td>
      <td>John Leguizamo</td>
      <td>201000</td>
      <td>36948322</td>
    </tr>
    <tr>
      <th>524</th>
      <td>Edward Scissorhands</td>
      <td>1990</td>
      <td>U</td>
      <td>105</td>
      <td>Drama, Fantasy, Romance</td>
      <td>7.9</td>
      <td>An artificial man, who was incompletely constr...</td>
      <td>74.00000</td>
      <td>Tim Burton</td>
      <td>Johnny Depp</td>
      <td>Winona Ryder</td>
      <td>Dianne Wiest</td>
      <td>Anthony Michael Hall</td>
      <td>447368</td>
      <td>56362352</td>
    </tr>
    <tr>
      <th>525</th>
      <td>My Left Foot: The Story of Christy Brown</td>
      <td>1989</td>
      <td>U</td>
      <td>103</td>
      <td>Biography, Drama</td>
      <td>7.9</td>
      <td>Christy Brown, born with cerebral palsy, learn...</td>
      <td>97.00000</td>
      <td>Jim Sheridan</td>
      <td>Daniel Day-Lewis</td>
      <td>Brenda Fricker</td>
      <td>Alison Whelan</td>
      <td>Kirsten Sheridan</td>
      <td>68076</td>
      <td>14743391</td>
    </tr>
    <tr>
      <th>526</th>
      <td>Crimes and Misdemeanors</td>
      <td>1989</td>
      <td>PG-13</td>
      <td>104</td>
      <td>Comedy, Drama</td>
      <td>7.9</td>
      <td>An ophthalmologist's mistress threatens to rev...</td>
      <td>77.00000</td>
      <td>Woody Allen</td>
      <td>Martin Landau</td>
      <td>Woody Allen</td>
      <td>Bill Bernstein</td>
      <td>Claire Bloom</td>
      <td>54670</td>
      <td>18254702</td>
    </tr>
    <tr>
      <th>527</th>
      <td>The Untouchables</td>
      <td>1987</td>
      <td>A</td>
      <td>119</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.9</td>
      <td>During the era of Prohibition in the United St...</td>
      <td>79.00000</td>
      <td>Brian De Palma</td>
      <td>Kevin Costner</td>
      <td>Sean Connery</td>
      <td>Robert De Niro</td>
      <td>Charles Martin Smith</td>
      <td>281842</td>
      <td>76270454</td>
    </tr>
    <tr>
      <th>528</th>
      <td>Hannah and Her Sisters</td>
      <td>1986</td>
      <td>PG-13</td>
      <td>107</td>
      <td>Comedy, Drama</td>
      <td>7.9</td>
      <td>Between two Thanksgivings two years apart, Han...</td>
      <td>90.00000</td>
      <td>Woody Allen</td>
      <td>Mia Farrow</td>
      <td>Dianne Wiest</td>
      <td>Michael Caine</td>
      <td>Barbara Hershey</td>
      <td>67176</td>
      <td>40084041</td>
    </tr>
    <tr>
      <th>529</th>
      <td>Brazil</td>
      <td>1985</td>
      <td>U</td>
      <td>132</td>
      <td>Drama, Sci-Fi</td>
      <td>7.9</td>
      <td>A bureaucrat in a dystopic society becomes an ...</td>
      <td>84.00000</td>
      <td>Terry Gilliam</td>
      <td>Jonathan Pryce</td>
      <td>Kim Greist</td>
      <td>Robert De Niro</td>
      <td>Katherine Helmond</td>
      <td>187567</td>
      <td>9929135</td>
    </tr>
    <tr>
      <th>530</th>
      <td>This Is Spinal Tap</td>
      <td>1984</td>
      <td>R</td>
      <td>82</td>
      <td>Comedy, Music</td>
      <td>7.9</td>
      <td>Spinal Tap, one of England's loudest bands, is...</td>
      <td>92.00000</td>
      <td>Rob Reiner</td>
      <td>Rob Reiner</td>
      <td>Michael McKean</td>
      <td>Christopher Guest</td>
      <td>Kimberly Stringer</td>
      <td>128812</td>
      <td>188751</td>
    </tr>
    <tr>
      <th>531</th>
      <td>A Christmas Story</td>
      <td>1983</td>
      <td>U</td>
      <td>93</td>
      <td>Comedy, Family</td>
      <td>7.9</td>
      <td>In the 1940s, a young boy named Ralphie attemp...</td>
      <td>77.00000</td>
      <td>Bob Clark</td>
      <td>Peter Billingsley</td>
      <td>Melinda Dillon</td>
      <td>Darren McGavin</td>
      <td>Scott Schwartz</td>
      <td>132947</td>
      <td>20605209</td>
    </tr>
    <tr>
      <th>532</th>
      <td>The Blues Brothers</td>
      <td>1980</td>
      <td>U</td>
      <td>133</td>
      <td>Action, Adventure, Comedy</td>
      <td>7.9</td>
      <td>Jake Blues, just released from prison, puts to...</td>
      <td>60.00000</td>
      <td>John Landis</td>
      <td>John Belushi</td>
      <td>Dan Aykroyd</td>
      <td>Cab Calloway</td>
      <td>John Candy</td>
      <td>183182</td>
      <td>57229890</td>
    </tr>
    <tr>
      <th>533</th>
      <td>Manhattan</td>
      <td>1979</td>
      <td>R</td>
      <td>96</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.9</td>
      <td>The life of a divorced television writer datin...</td>
      <td>83.00000</td>
      <td>Woody Allen</td>
      <td>Woody Allen</td>
      <td>Diane Keaton</td>
      <td>Mariel Hemingway</td>
      <td>Michael Murphy</td>
      <td>131436</td>
      <td>45700000</td>
    </tr>
    <tr>
      <th>534</th>
      <td>All That Jazz</td>
      <td>1979</td>
      <td>A</td>
      <td>123</td>
      <td>Drama, Music, Musical</td>
      <td>7.9</td>
      <td>Director/choreographer Bob Fosse tells his own...</td>
      <td>72.00000</td>
      <td>Bob Fosse</td>
      <td>Roy Scheider</td>
      <td>Jessica Lange</td>
      <td>Ann Reinking</td>
      <td>Leland Palmer</td>
      <td>28223</td>
      <td>37823676</td>
    </tr>
    <tr>
      <th>535</th>
      <td>Dawn of the Dead</td>
      <td>1978</td>
      <td>A</td>
      <td>127</td>
      <td>Action, Adventure, Horror</td>
      <td>7.9</td>
      <td>Following an ever-growing epidemic of zombies ...</td>
      <td>71.00000</td>
      <td>George A. Romero</td>
      <td>David Emge</td>
      <td>Ken Foree</td>
      <td>Scott H. Reiniger</td>
      <td>Gaylen Ross</td>
      <td>111512</td>
      <td>5100000</td>
    </tr>
    <tr>
      <th>536</th>
      <td>All the President's Men</td>
      <td>1976</td>
      <td>U</td>
      <td>138</td>
      <td>Biography, Drama, History</td>
      <td>7.9</td>
      <td>"The Washington Post" reporters Bob Woodward a...</td>
      <td>84.00000</td>
      <td>Alan J. Pakula</td>
      <td>Dustin Hoffman</td>
      <td>Robert Redford</td>
      <td>Jack Warden</td>
      <td>Martin Balsam</td>
      <td>103031</td>
      <td>70600000</td>
    </tr>
    <tr>
      <th>537</th>
      <td>La montaña sagrada</td>
      <td>1973</td>
      <td>R</td>
      <td>114</td>
      <td>Adventure, Drama, Fantasy</td>
      <td>7.9</td>
      <td>In a corrupt, greed-fueled world, a powerful a...</td>
      <td>76.00000</td>
      <td>Alejandro Jodorowsky</td>
      <td>Alejandro Jodorowsky</td>
      <td>Horacio Salinas</td>
      <td>Zamira Saunders</td>
      <td>Juan Ferrara</td>
      <td>37183</td>
      <td>61001</td>
    </tr>
    <tr>
      <th>538</th>
      <td>Amarcord</td>
      <td>1973</td>
      <td>R</td>
      <td>123</td>
      <td>Comedy, Drama, Family</td>
      <td>7.9</td>
      <td>A series of comedic and nostalgic vignettes se...</td>
      <td>77.97153</td>
      <td>Federico Fellini</td>
      <td>Magali Noël</td>
      <td>Bruno Zanin</td>
      <td>Pupella Maggio</td>
      <td>Armando Brancia</td>
      <td>39897</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>539</th>
      <td>Le charme discret de la bourgeoisie</td>
      <td>1972</td>
      <td>PG</td>
      <td>102</td>
      <td>Comedy</td>
      <td>7.9</td>
      <td>A surreal, virtually plotless series of dreams...</td>
      <td>93.00000</td>
      <td>Luis Buñuel</td>
      <td>Fernando Rey</td>
      <td>Delphine Seyrig</td>
      <td>Paul Frankeur</td>
      <td>Bulle Ogier</td>
      <td>38737</td>
      <td>198809</td>
    </tr>
    <tr>
      <th>540</th>
      <td>Aguirre, der Zorn Gottes</td>
      <td>1972</td>
      <td>Unknown</td>
      <td>95</td>
      <td>Action, Adventure, Biography</td>
      <td>7.9</td>
      <td>In the 16th century, the ruthless and insane D...</td>
      <td>77.97153</td>
      <td>Werner Herzog</td>
      <td>Klaus Kinski</td>
      <td>Ruy Guerra</td>
      <td>Helena Rojo</td>
      <td>Del Negro</td>
      <td>52397</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>541</th>
      <td>Harold and Maude</td>
      <td>1971</td>
      <td>PG</td>
      <td>91</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.9</td>
      <td>Young, rich, and obsessed with death, Harold f...</td>
      <td>62.00000</td>
      <td>Hal Ashby</td>
      <td>Ruth Gordon</td>
      <td>Bud Cort</td>
      <td>Vivian Pickles</td>
      <td>Cyril Cusack</td>
      <td>70826</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>542</th>
      <td>Patton</td>
      <td>1970</td>
      <td>U</td>
      <td>172</td>
      <td>Biography, Drama, War</td>
      <td>7.9</td>
      <td>The World War II phase of the career of contro...</td>
      <td>91.00000</td>
      <td>Franklin J. Schaffner</td>
      <td>George C. Scott</td>
      <td>Karl Malden</td>
      <td>Stephen Young</td>
      <td>Michael Strong</td>
      <td>93741</td>
      <td>61700000</td>
    </tr>
    <tr>
      <th>543</th>
      <td>The Wild Bunch</td>
      <td>1969</td>
      <td>A</td>
      <td>145</td>
      <td>Action, Adventure, Western</td>
      <td>7.9</td>
      <td>An aging group of outlaws look for one last bi...</td>
      <td>97.00000</td>
      <td>Sam Peckinpah</td>
      <td>William Holden</td>
      <td>Ernest Borgnine</td>
      <td>Robert Ryan</td>
      <td>Edmond O'Brien</td>
      <td>77401</td>
      <td>12064472</td>
    </tr>
    <tr>
      <th>544</th>
      <td>Night of the Living Dead</td>
      <td>1968</td>
      <td>Unknown</td>
      <td>96</td>
      <td>Horror, Thriller</td>
      <td>7.9</td>
      <td>A ragtag group of Pennsylvanians barricade the...</td>
      <td>89.00000</td>
      <td>George A. Romero</td>
      <td>Duane Jones</td>
      <td>Judith O'Dea</td>
      <td>Karl Hardman</td>
      <td>Marilyn Eastman</td>
      <td>116557</td>
      <td>89029</td>
    </tr>
    <tr>
      <th>545</th>
      <td>The Lion in Winter</td>
      <td>1968</td>
      <td>PG</td>
      <td>134</td>
      <td>Biography, Drama, History</td>
      <td>7.9</td>
      <td>1183 A.D.: King Henry II's three sons all want...</td>
      <td>77.97153</td>
      <td>Anthony Harvey</td>
      <td>Peter O'Toole</td>
      <td>Katharine Hepburn</td>
      <td>Anthony Hopkins</td>
      <td>John Castle</td>
      <td>29003</td>
      <td>22276975</td>
    </tr>
    <tr>
      <th>546</th>
      <td>In the Heat of the Night</td>
      <td>1967</td>
      <td>U</td>
      <td>110</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.9</td>
      <td>A black police detective is asked to investiga...</td>
      <td>75.00000</td>
      <td>Norman Jewison</td>
      <td>Sidney Poitier</td>
      <td>Rod Steiger</td>
      <td>Warren Oates</td>
      <td>Lee Grant</td>
      <td>67804</td>
      <td>24379978</td>
    </tr>
    <tr>
      <th>547</th>
      <td>Charade</td>
      <td>1963</td>
      <td>U</td>
      <td>113</td>
      <td>Comedy, Mystery, Romance</td>
      <td>7.9</td>
      <td>Romance and suspense ensue in Paris as a woman...</td>
      <td>83.00000</td>
      <td>Stanley Donen</td>
      <td>Cary Grant</td>
      <td>Audrey Hepburn</td>
      <td>Walter Matthau</td>
      <td>James Coburn</td>
      <td>68689</td>
      <td>13474588</td>
    </tr>
    <tr>
      <th>548</th>
      <td>The Manchurian Candidate</td>
      <td>1962</td>
      <td>PG-13</td>
      <td>126</td>
      <td>Drama, Thriller</td>
      <td>7.9</td>
      <td>A former prisoner of war is brainwashed as an ...</td>
      <td>94.00000</td>
      <td>John Frankenheimer</td>
      <td>Frank Sinatra</td>
      <td>Laurence Harvey</td>
      <td>Janet Leigh</td>
      <td>Angela Lansbury</td>
      <td>71122</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>549</th>
      <td>Spartacus</td>
      <td>1960</td>
      <td>A</td>
      <td>197</td>
      <td>Adventure, Biography, Drama</td>
      <td>7.9</td>
      <td>The slave Spartacus leads a violent revolt aga...</td>
      <td>87.00000</td>
      <td>Stanley Kubrick</td>
      <td>Kirk Douglas</td>
      <td>Laurence Olivier</td>
      <td>Jean Simmons</td>
      <td>Charles Laughton</td>
      <td>124339</td>
      <td>30000000</td>
    </tr>
    <tr>
      <th>550</th>
      <td>L'avventura</td>
      <td>1960</td>
      <td>U</td>
      <td>144</td>
      <td>Drama, Mystery</td>
      <td>7.9</td>
      <td>A woman disappears during a Mediterranean boat...</td>
      <td>77.97153</td>
      <td>Michelangelo Antonioni</td>
      <td>Gabriele Ferzetti</td>
      <td>Monica Vitti</td>
      <td>Lea Massari</td>
      <td>Dominique Blanchar</td>
      <td>26542</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>551</th>
      <td>Hiroshima mon amour</td>
      <td>1959</td>
      <td>Unknown</td>
      <td>90</td>
      <td>Drama, Romance</td>
      <td>7.9</td>
      <td>A French actress filming an anti-war film in H...</td>
      <td>77.97153</td>
      <td>Alain Resnais</td>
      <td>Emmanuelle Riva</td>
      <td>Eiji Okada</td>
      <td>Stella Dassas</td>
      <td>Pierre Barbaud</td>
      <td>28421</td>
      <td>88300</td>
    </tr>
    <tr>
      <th>552</th>
      <td>The Ten Commandments</td>
      <td>1956</td>
      <td>U</td>
      <td>220</td>
      <td>Adventure, Drama</td>
      <td>7.9</td>
      <td>Moses, an Egyptian Prince, learns of his true ...</td>
      <td>77.97153</td>
      <td>Cecil B. DeMille</td>
      <td>Charlton Heston</td>
      <td>Yul Brynner</td>
      <td>Anne Baxter</td>
      <td>Edward G. Robinson</td>
      <td>63560</td>
      <td>93740000</td>
    </tr>
    <tr>
      <th>553</th>
      <td>The Searchers</td>
      <td>1956</td>
      <td>Passed</td>
      <td>119</td>
      <td>Adventure, Drama, Western</td>
      <td>7.9</td>
      <td>An American Civil War veteran embarks on a jou...</td>
      <td>94.00000</td>
      <td>John Ford</td>
      <td>John Wayne</td>
      <td>Jeffrey Hunter</td>
      <td>Vera Miles</td>
      <td>Ward Bond</td>
      <td>80316</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>554</th>
      <td>East of Eden</td>
      <td>1955</td>
      <td>U</td>
      <td>118</td>
      <td>Drama</td>
      <td>7.9</td>
      <td>Two brothers struggle to maintain their strict...</td>
      <td>72.00000</td>
      <td>Elia Kazan</td>
      <td>James Dean</td>
      <td>Raymond Massey</td>
      <td>Julie Harris</td>
      <td>Burl Ives</td>
      <td>40313</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>555</th>
      <td>High Noon</td>
      <td>1952</td>
      <td>PG</td>
      <td>85</td>
      <td>Drama, Thriller, Western</td>
      <td>7.9</td>
      <td>A town Marshal, despite the disagreements of h...</td>
      <td>89.00000</td>
      <td>Fred Zinnemann</td>
      <td>Gary Cooper</td>
      <td>Grace Kelly</td>
      <td>Thomas Mitchell</td>
      <td>Lloyd Bridges</td>
      <td>97222</td>
      <td>9450000</td>
    </tr>
    <tr>
      <th>556</th>
      <td>Strangers on a Train</td>
      <td>1951</td>
      <td>A</td>
      <td>101</td>
      <td>Crime, Film-Noir, Thriller</td>
      <td>7.9</td>
      <td>A psychopath forces a tennis star to comply wi...</td>
      <td>88.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Farley Granger</td>
      <td>Robert Walker</td>
      <td>Ruth Roman</td>
      <td>Leo G. Carroll</td>
      <td>123341</td>
      <td>7630000</td>
    </tr>
    <tr>
      <th>557</th>
      <td>Harvey</td>
      <td>1950</td>
      <td>Approved</td>
      <td>104</td>
      <td>Comedy, Drama, Fantasy</td>
      <td>7.9</td>
      <td>Due to his insistence that he has an invisible...</td>
      <td>77.97153</td>
      <td>Henry Koster</td>
      <td>James Stewart</td>
      <td>Wallace Ford</td>
      <td>William H. Lynn</td>
      <td>Victoria Horne</td>
      <td>52573</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>558</th>
      <td>Miracle on 34th Street</td>
      <td>1947</td>
      <td>Unknown</td>
      <td>96</td>
      <td>Comedy, Drama, Family</td>
      <td>7.9</td>
      <td>When a nice old man who claims to be Santa Cla...</td>
      <td>88.00000</td>
      <td>George Seaton</td>
      <td>Edmund Gwenn</td>
      <td>Maureen O'Hara</td>
      <td>John Payne</td>
      <td>Gene Lockhart</td>
      <td>41625</td>
      <td>2650000</td>
    </tr>
    <tr>
      <th>559</th>
      <td>Notorious</td>
      <td>1946</td>
      <td>U</td>
      <td>102</td>
      <td>Drama, Film-Noir, Romance</td>
      <td>7.9</td>
      <td>A woman is asked to spy on a group of Nazi fri...</td>
      <td>100.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Cary Grant</td>
      <td>Ingrid Bergman</td>
      <td>Claude Rains</td>
      <td>Louis Calhern</td>
      <td>92306</td>
      <td>10464000</td>
    </tr>
    <tr>
      <th>560</th>
      <td>The Big Sleep</td>
      <td>1946</td>
      <td>Passed</td>
      <td>114</td>
      <td>Crime, Film-Noir, Mystery</td>
      <td>7.9</td>
      <td>Private detective Philip Marlowe is hired by a...</td>
      <td>77.97153</td>
      <td>Howard Hawks</td>
      <td>Humphrey Bogart</td>
      <td>Lauren Bacall</td>
      <td>John Ridgely</td>
      <td>Martha Vickers</td>
      <td>78796</td>
      <td>6540000</td>
    </tr>
    <tr>
      <th>561</th>
      <td>The Lost Weekend</td>
      <td>1945</td>
      <td>Passed</td>
      <td>101</td>
      <td>Drama, Film-Noir</td>
      <td>7.9</td>
      <td>The desperate life of a chronic alcoholic is f...</td>
      <td>77.97153</td>
      <td>Billy Wilder</td>
      <td>Ray Milland</td>
      <td>Jane Wyman</td>
      <td>Phillip Terry</td>
      <td>Howard Da Silva</td>
      <td>33549</td>
      <td>9460000</td>
    </tr>
    <tr>
      <th>562</th>
      <td>The Philadelphia Story</td>
      <td>1940</td>
      <td>Unknown</td>
      <td>112</td>
      <td>Comedy, Romance</td>
      <td>7.9</td>
      <td>When a rich woman's ex-husband and a tabloid-t...</td>
      <td>96.00000</td>
      <td>George Cukor</td>
      <td>Cary Grant</td>
      <td>Katharine Hepburn</td>
      <td>James Stewart</td>
      <td>Ruth Hussey</td>
      <td>63550</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>563</th>
      <td>His Girl Friday</td>
      <td>1940</td>
      <td>Passed</td>
      <td>92</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.9</td>
      <td>A newspaper editor uses every trick in the boo...</td>
      <td>77.97153</td>
      <td>Howard Hawks</td>
      <td>Cary Grant</td>
      <td>Rosalind Russell</td>
      <td>Ralph Bellamy</td>
      <td>Gene Lockhart</td>
      <td>53667</td>
      <td>296000</td>
    </tr>
    <tr>
      <th>564</th>
      <td>The Adventures of Robin Hood</td>
      <td>1938</td>
      <td>PG</td>
      <td>102</td>
      <td>Action, Adventure, Romance</td>
      <td>7.9</td>
      <td>When Prince John and the Norman Lords begin op...</td>
      <td>97.00000</td>
      <td>Michael Curtiz</td>
      <td>William Keighley</td>
      <td>Errol Flynn</td>
      <td>Olivia de Havilland</td>
      <td>Basil Rathbone</td>
      <td>47175</td>
      <td>3981000</td>
    </tr>
    <tr>
      <th>565</th>
      <td>A Night at the Opera</td>
      <td>1935</td>
      <td>Passed</td>
      <td>96</td>
      <td>Comedy, Music, Musical</td>
      <td>7.9</td>
      <td>A sly business manager and two wacky friends o...</td>
      <td>77.97153</td>
      <td>Sam Wood</td>
      <td>Edmund Goulding</td>
      <td>Groucho Marx</td>
      <td>Chico Marx</td>
      <td>Harpo Marx</td>
      <td>30580</td>
      <td>2537520</td>
    </tr>
    <tr>
      <th>566</th>
      <td>King Kong</td>
      <td>1933</td>
      <td>Passed</td>
      <td>100</td>
      <td>Adventure, Horror, Sci-Fi</td>
      <td>7.9</td>
      <td>A film crew goes to a tropical island for an e...</td>
      <td>90.00000</td>
      <td>Merian C. Cooper</td>
      <td>Ernest B. Schoedsack</td>
      <td>Fay Wray</td>
      <td>Robert Armstrong</td>
      <td>Bruce Cabot</td>
      <td>78991</td>
      <td>10000000</td>
    </tr>
    <tr>
      <th>567</th>
      <td>Freaks</td>
      <td>1932</td>
      <td>Unknown</td>
      <td>64</td>
      <td>Drama, Horror</td>
      <td>7.9</td>
      <td>A circus' beautiful trapeze artist agrees to m...</td>
      <td>80.00000</td>
      <td>Tod Browning</td>
      <td>Wallace Ford</td>
      <td>Leila Hyams</td>
      <td>Olga Baclanova</td>
      <td>Roscoe Ates</td>
      <td>42117</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>568</th>
      <td>Nosferatu</td>
      <td>1922</td>
      <td>Unknown</td>
      <td>94</td>
      <td>Fantasy, Horror</td>
      <td>7.9</td>
      <td>Vampire Count Orlok expresses interest in a ne...</td>
      <td>77.97153</td>
      <td>F.W. Murnau</td>
      <td>Max Schreck</td>
      <td>Alexander Granach</td>
      <td>Gustav von Wangenheim</td>
      <td>Greta Schröder</td>
      <td>88794</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>569</th>
      <td>The Gentlemen</td>
      <td>2019</td>
      <td>A</td>
      <td>113</td>
      <td>Action, Comedy, Crime</td>
      <td>7.8</td>
      <td>An American expat tries to sell off his highly...</td>
      <td>51.00000</td>
      <td>Guy Ritchie</td>
      <td>Matthew McConaughey</td>
      <td>Charlie Hunnam</td>
      <td>Michelle Dockery</td>
      <td>Jeremy Strong</td>
      <td>237392</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>570</th>
      <td>Raazi</td>
      <td>2018</td>
      <td>UA</td>
      <td>138</td>
      <td>Action, Drama, Thriller</td>
      <td>7.8</td>
      <td>A Kashmiri woman agrees to marry a Pakistani a...</td>
      <td>77.97153</td>
      <td>Meghna Gulzar</td>
      <td>Alia Bhatt</td>
      <td>Vicky Kaushal</td>
      <td>Rajit Kapoor</td>
      <td>Shishir Sharma</td>
      <td>25344</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>571</th>
      <td>Sound of Metal</td>
      <td>2019</td>
      <td>R</td>
      <td>120</td>
      <td>Drama, Music</td>
      <td>7.8</td>
      <td>A heavy-metal drummer's life is thrown into fr...</td>
      <td>81.00000</td>
      <td>Darius Marder</td>
      <td>Riz Ahmed</td>
      <td>Olivia Cooke</td>
      <td>Paul Raci</td>
      <td>Lauren Ridloff</td>
      <td>27187</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>572</th>
      <td>Forushande</td>
      <td>2016</td>
      <td>UA</td>
      <td>124</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>While both participating in a production of "D...</td>
      <td>85.00000</td>
      <td>Asghar Farhadi</td>
      <td>Shahab Hosseini</td>
      <td>Taraneh Alidoosti</td>
      <td>Babak Karimi</td>
      <td>Mina Sadati</td>
      <td>51240</td>
      <td>2402067</td>
    </tr>
    <tr>
      <th>573</th>
      <td>Dunkirk</td>
      <td>2017</td>
      <td>UA</td>
      <td>106</td>
      <td>Action, Drama, History</td>
      <td>7.8</td>
      <td>Allied soldiers from Belgium, the British Empi...</td>
      <td>94.00000</td>
      <td>Christopher Nolan</td>
      <td>Fionn Whitehead</td>
      <td>Barry Keoghan</td>
      <td>Mark Rylance</td>
      <td>Tom Hardy</td>
      <td>555092</td>
      <td>188373161</td>
    </tr>
    <tr>
      <th>574</th>
      <td>Perfetti sconosciuti</td>
      <td>2016</td>
      <td>Unknown</td>
      <td>96</td>
      <td>Comedy, Drama</td>
      <td>7.8</td>
      <td>Seven long-time friends get together for a din...</td>
      <td>77.97153</td>
      <td>Paolo Genovese</td>
      <td>Giuseppe Battiston</td>
      <td>Anna Foglietta</td>
      <td>Marco Giallini</td>
      <td>Edoardo Leo</td>
      <td>57168</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>575</th>
      <td>Hidden Figures</td>
      <td>2016</td>
      <td>UA</td>
      <td>127</td>
      <td>Biography, Drama, History</td>
      <td>7.8</td>
      <td>The story of a team of female African-American...</td>
      <td>74.00000</td>
      <td>Theodore Melfi</td>
      <td>Taraji P. Henson</td>
      <td>Octavia Spencer</td>
      <td>Janelle Monáe</td>
      <td>Kevin Costner</td>
      <td>200876</td>
      <td>169607287</td>
    </tr>
    <tr>
      <th>576</th>
      <td>Paddington 2</td>
      <td>2017</td>
      <td>U</td>
      <td>103</td>
      <td>Adventure, Comedy, Family</td>
      <td>7.8</td>
      <td>Paddington (Ben Whishaw), now happily settled ...</td>
      <td>88.00000</td>
      <td>Paul King</td>
      <td>Ben Whishaw</td>
      <td>Hugh Grant</td>
      <td>Hugh Bonneville</td>
      <td>Sally Hawkins</td>
      <td>61594</td>
      <td>40442052</td>
    </tr>
    <tr>
      <th>577</th>
      <td>Udta Punjab</td>
      <td>2016</td>
      <td>A</td>
      <td>148</td>
      <td>Action, Crime, Drama</td>
      <td>7.8</td>
      <td>A story that revolves around drug abuse in the...</td>
      <td>77.97153</td>
      <td>Abhishek Chaubey</td>
      <td>Shahid Kapoor</td>
      <td>Alia Bhatt</td>
      <td>Kareena Kapoor</td>
      <td>Diljit Dosanjh</td>
      <td>27175</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>578</th>
      <td>Kubo and the Two Strings</td>
      <td>2016</td>
      <td>PG</td>
      <td>101</td>
      <td>Animation, Action, Adventure</td>
      <td>7.8</td>
      <td>A young boy named Kubo must locate a magical s...</td>
      <td>84.00000</td>
      <td>Travis Knight</td>
      <td>Charlize Theron</td>
      <td>Art Parkinson</td>
      <td>Matthew McConaughey</td>
      <td>Ralph Fiennes</td>
      <td>118035</td>
      <td>48023088</td>
    </tr>
    <tr>
      <th>579</th>
      <td>M.S. Dhoni: The Untold Story</td>
      <td>2016</td>
      <td>U</td>
      <td>184</td>
      <td>Biography, Drama, Sport</td>
      <td>7.8</td>
      <td>The untold story of Mahendra Singh Dhoni's jou...</td>
      <td>77.97153</td>
      <td>Neeraj Pandey</td>
      <td>Sushant Singh Rajput</td>
      <td>Kiara Advani</td>
      <td>Anupam Kher</td>
      <td>Disha Patani</td>
      <td>40416</td>
      <td>1782795</td>
    </tr>
    <tr>
      <th>580</th>
      <td>Manchester by the Sea</td>
      <td>2016</td>
      <td>UA</td>
      <td>137</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>A depressed uncle is asked to take care of his...</td>
      <td>96.00000</td>
      <td>Kenneth Lonergan</td>
      <td>Casey Affleck</td>
      <td>Michelle Williams</td>
      <td>Kyle Chandler</td>
      <td>Lucas Hedges</td>
      <td>246963</td>
      <td>47695120</td>
    </tr>
    <tr>
      <th>581</th>
      <td>Under sandet</td>
      <td>2015</td>
      <td>R</td>
      <td>100</td>
      <td>Drama, History, War</td>
      <td>7.8</td>
      <td>In post-World War II Denmark, a group of young...</td>
      <td>75.00000</td>
      <td>Martin Zandvliet</td>
      <td>Roland Møller</td>
      <td>Louis Hofmann</td>
      <td>Joel Basman</td>
      <td>Mikkel Boe Følsgaard</td>
      <td>35539</td>
      <td>435266</td>
    </tr>
    <tr>
      <th>582</th>
      <td>Rogue One</td>
      <td>2016</td>
      <td>UA</td>
      <td>133</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.8</td>
      <td>The daughter of an Imperial scientist joins th...</td>
      <td>65.00000</td>
      <td>Gareth Edwards</td>
      <td>Felicity Jones</td>
      <td>Diego Luna</td>
      <td>Alan Tudyk</td>
      <td>Donnie Yen</td>
      <td>556608</td>
      <td>532177324</td>
    </tr>
    <tr>
      <th>583</th>
      <td>Captain America: Civil War</td>
      <td>2016</td>
      <td>UA</td>
      <td>147</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.8</td>
      <td>Political involvement in the Avengers' affairs...</td>
      <td>75.00000</td>
      <td>Anthony Russo</td>
      <td>Joe Russo</td>
      <td>Chris Evans</td>
      <td>Robert Downey Jr.</td>
      <td>Scarlett Johansson</td>
      <td>663649</td>
      <td>408084349</td>
    </tr>
    <tr>
      <th>584</th>
      <td>The Hateful Eight</td>
      <td>2015</td>
      <td>A</td>
      <td>168</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.8</td>
      <td>In the dead of a Wyoming winter, a bounty hunt...</td>
      <td>68.00000</td>
      <td>Quentin Tarantino</td>
      <td>Samuel L. Jackson</td>
      <td>Kurt Russell</td>
      <td>Jennifer Jason Leigh</td>
      <td>Walton Goggins</td>
      <td>517059</td>
      <td>54117416</td>
    </tr>
    <tr>
      <th>585</th>
      <td>Little Women</td>
      <td>2019</td>
      <td>U</td>
      <td>135</td>
      <td>Drama, Romance</td>
      <td>7.8</td>
      <td>Jo March reflects back and forth on her life, ...</td>
      <td>91.00000</td>
      <td>Greta Gerwig</td>
      <td>Saoirse Ronan</td>
      <td>Emma Watson</td>
      <td>Florence Pugh</td>
      <td>Eliza Scanlen</td>
      <td>143250</td>
      <td>108101214</td>
    </tr>
    <tr>
      <th>586</th>
      <td>Loving Vincent</td>
      <td>2017</td>
      <td>UA</td>
      <td>94</td>
      <td>Animation, Biography, Crime</td>
      <td>7.8</td>
      <td>In a story depicted in oil painted animation, ...</td>
      <td>62.00000</td>
      <td>Dorota Kobiela</td>
      <td>Hugh Welchman</td>
      <td>Douglas Booth</td>
      <td>Jerome Flynn</td>
      <td>Robert Gulaczyk</td>
      <td>50778</td>
      <td>6735118</td>
    </tr>
    <tr>
      <th>587</th>
      <td>Pride</td>
      <td>2014</td>
      <td>R</td>
      <td>119</td>
      <td>Biography, Comedy, Drama</td>
      <td>7.8</td>
      <td>U.K. gay activists work to help miners during ...</td>
      <td>79.00000</td>
      <td>Matthew Warchus</td>
      <td>Bill Nighy</td>
      <td>Imelda Staunton</td>
      <td>Dominic West</td>
      <td>Paddy Considine</td>
      <td>51841</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>588</th>
      <td>Le passé</td>
      <td>2013</td>
      <td>PG-13</td>
      <td>130</td>
      <td>Drama, Mystery</td>
      <td>7.8</td>
      <td>An Iranian man deserts his French wife and her...</td>
      <td>85.00000</td>
      <td>Asghar Farhadi</td>
      <td>Bérénice Bejo</td>
      <td>Tahar Rahim</td>
      <td>Ali Mosaffa</td>
      <td>Pauline Burlet</td>
      <td>45002</td>
      <td>1330596</td>
    </tr>
    <tr>
      <th>589</th>
      <td>La grande bellezza</td>
      <td>2013</td>
      <td>Unknown</td>
      <td>141</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>Jep Gambardella has seduced his way through th...</td>
      <td>86.00000</td>
      <td>Paolo Sorrentino</td>
      <td>Toni Servillo</td>
      <td>Carlo Verdone</td>
      <td>Sabrina Ferilli</td>
      <td>Carlo Buccirosso</td>
      <td>81125</td>
      <td>2852400</td>
    </tr>
    <tr>
      <th>590</th>
      <td>The Lunchbox</td>
      <td>2013</td>
      <td>U</td>
      <td>104</td>
      <td>Drama, Romance</td>
      <td>7.8</td>
      <td>A mistaken delivery in Mumbai's famously effic...</td>
      <td>76.00000</td>
      <td>Ritesh Batra</td>
      <td>Irrfan Khan</td>
      <td>Nimrat Kaur</td>
      <td>Nawazuddin Siddiqui</td>
      <td>Lillete Dubey</td>
      <td>50523</td>
      <td>4231500</td>
    </tr>
    <tr>
      <th>591</th>
      <td>Vicky Donor</td>
      <td>2012</td>
      <td>UA</td>
      <td>126</td>
      <td>Comedy, Romance</td>
      <td>7.8</td>
      <td>A man is brought in by an infertility doctor t...</td>
      <td>77.97153</td>
      <td>Shoojit Sircar</td>
      <td>Ayushmann Khurrana</td>
      <td>Yami Gautam</td>
      <td>Annu Kapoor</td>
      <td>Dolly Ahluwalia</td>
      <td>39710</td>
      <td>169209</td>
    </tr>
    <tr>
      <th>592</th>
      <td>Big Hero 6</td>
      <td>2014</td>
      <td>U</td>
      <td>102</td>
      <td>Animation, Action, Adventure</td>
      <td>7.8</td>
      <td>A special bond develops between plus-sized inf...</td>
      <td>74.00000</td>
      <td>Don Hall</td>
      <td>Chris Williams</td>
      <td>Ryan Potter</td>
      <td>Scott Adsit</td>
      <td>Jamie Chung</td>
      <td>410983</td>
      <td>222527828</td>
    </tr>
    <tr>
      <th>593</th>
      <td>About Time</td>
      <td>2013</td>
      <td>R</td>
      <td>123</td>
      <td>Comedy, Drama, Fantasy</td>
      <td>7.8</td>
      <td>At the age of 21, Tim discovers he can travel ...</td>
      <td>55.00000</td>
      <td>Richard Curtis</td>
      <td>Domhnall Gleeson</td>
      <td>Rachel McAdams</td>
      <td>Bill Nighy</td>
      <td>Lydia Wilson</td>
      <td>303032</td>
      <td>15322921</td>
    </tr>
    <tr>
      <th>594</th>
      <td>English Vinglish</td>
      <td>2012</td>
      <td>U</td>
      <td>134</td>
      <td>Comedy, Drama, Family</td>
      <td>7.8</td>
      <td>A quiet, sweet tempered housewife endures smal...</td>
      <td>77.97153</td>
      <td>Gauri Shinde</td>
      <td>Sridevi</td>
      <td>Adil Hussain</td>
      <td>Mehdi Nebbou</td>
      <td>Priya Anand</td>
      <td>33618</td>
      <td>1670773</td>
    </tr>
    <tr>
      <th>595</th>
      <td>Kaze tachinu</td>
      <td>2013</td>
      <td>PG-13</td>
      <td>126</td>
      <td>Animation, Biography, Drama</td>
      <td>7.8</td>
      <td>A look at the life of Jiro Horikoshi, the man ...</td>
      <td>83.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Hideaki Anno</td>
      <td>Hidetoshi Nishijima</td>
      <td>Miori Takimoto</td>
      <td>Masahiko Nishimura</td>
      <td>73690</td>
      <td>5209580</td>
    </tr>
    <tr>
      <th>596</th>
      <td>Toy Story 4</td>
      <td>2019</td>
      <td>U</td>
      <td>100</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.8</td>
      <td>When a new toy called "Forky" joins Woody and ...</td>
      <td>84.00000</td>
      <td>Josh Cooley</td>
      <td>Tom Hanks</td>
      <td>Tim Allen</td>
      <td>Annie Potts</td>
      <td>Tony Hale</td>
      <td>203177</td>
      <td>434038008</td>
    </tr>
    <tr>
      <th>597</th>
      <td>La migliore offerta</td>
      <td>2013</td>
      <td>R</td>
      <td>131</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.8</td>
      <td>A lonely art expert working for a mysterious a...</td>
      <td>49.00000</td>
      <td>Giuseppe Tornatore</td>
      <td>Geoffrey Rush</td>
      <td>Jim Sturgess</td>
      <td>Sylvia Hoeks</td>
      <td>Donald Sutherland</td>
      <td>108399</td>
      <td>85433</td>
    </tr>
    <tr>
      <th>598</th>
      <td>Moonrise Kingdom</td>
      <td>2012</td>
      <td>A</td>
      <td>94</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.8</td>
      <td>A pair of young lovers flee their New England ...</td>
      <td>84.00000</td>
      <td>Wes Anderson</td>
      <td>Jared Gilman</td>
      <td>Kara Hayward</td>
      <td>Bruce Willis</td>
      <td>Bill Murray</td>
      <td>318789</td>
      <td>45512466</td>
    </tr>
    <tr>
      <th>599</th>
      <td>How to Train Your Dragon 2</td>
      <td>2014</td>
      <td>U</td>
      <td>102</td>
      <td>Animation, Action, Adventure</td>
      <td>7.8</td>
      <td>When Hiccup and Toothless discover an ice cave...</td>
      <td>76.00000</td>
      <td>Dean DeBlois</td>
      <td>Jay Baruchel</td>
      <td>Cate Blanchett</td>
      <td>Gerard Butler</td>
      <td>Craig Ferguson</td>
      <td>305611</td>
      <td>177002924</td>
    </tr>
    <tr>
      <th>600</th>
      <td>The Big Short</td>
      <td>2015</td>
      <td>A</td>
      <td>130</td>
      <td>Biography, Comedy, Drama</td>
      <td>7.8</td>
      <td>In 2006-2007 a group of investors bet against ...</td>
      <td>81.00000</td>
      <td>Adam McKay</td>
      <td>Christian Bale</td>
      <td>Steve Carell</td>
      <td>Ryan Gosling</td>
      <td>Brad Pitt</td>
      <td>362942</td>
      <td>70259870</td>
    </tr>
    <tr>
      <th>601</th>
      <td>Kokuhaku</td>
      <td>2010</td>
      <td>Unknown</td>
      <td>106</td>
      <td>Drama, Thriller</td>
      <td>7.8</td>
      <td>A psychological thriller of a grieving mother ...</td>
      <td>77.97153</td>
      <td>Tetsuya Nakashima</td>
      <td>Takako Matsu</td>
      <td>Yoshino Kimura</td>
      <td>Masaki Okada</td>
      <td>Yukito Nishii</td>
      <td>35713</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>602</th>
      <td>Ang-ma-reul bo-at-da</td>
      <td>2010</td>
      <td>Unknown</td>
      <td>144</td>
      <td>Action, Crime, Drama</td>
      <td>7.8</td>
      <td>A secret agent exacts revenge on a serial kill...</td>
      <td>67.00000</td>
      <td>Jee-woon Kim</td>
      <td>Lee Byung-Hun</td>
      <td>Choi Min-sik</td>
      <td>Jeon Gook-Hwan</td>
      <td>Ho-jin Chun</td>
      <td>111252</td>
      <td>128392</td>
    </tr>
    <tr>
      <th>603</th>
      <td>The Girl with the Dragon Tattoo</td>
      <td>2011</td>
      <td>R</td>
      <td>158</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.8</td>
      <td>Journalist Mikael Blomkvist is aided in his se...</td>
      <td>71.00000</td>
      <td>David Fincher</td>
      <td>Daniel Craig</td>
      <td>Rooney Mara</td>
      <td>Christopher Plummer</td>
      <td>Stellan Skarsgård</td>
      <td>423010</td>
      <td>102515793</td>
    </tr>
    <tr>
      <th>604</th>
      <td>Captain Phillips</td>
      <td>2013</td>
      <td>UA</td>
      <td>134</td>
      <td>Adventure, Biography, Crime</td>
      <td>7.8</td>
      <td>The true story of Captain Richard Phillips and...</td>
      <td>82.00000</td>
      <td>Paul Greengrass</td>
      <td>Tom Hanks</td>
      <td>Barkhad Abdi</td>
      <td>Barkhad Abdirahman</td>
      <td>Catherine Keener</td>
      <td>421244</td>
      <td>107100855</td>
    </tr>
    <tr>
      <th>605</th>
      <td>Ajeossi</td>
      <td>2010</td>
      <td>R</td>
      <td>119</td>
      <td>Action, Crime, Drama</td>
      <td>7.8</td>
      <td>A quiet pawnshop keeper with a violent past ta...</td>
      <td>77.97153</td>
      <td>Jeong-beom Lee</td>
      <td>Won Bin</td>
      <td>Sae-ron Kim</td>
      <td>Tae-hoon Kim</td>
      <td>Hee-won Kim</td>
      <td>62848</td>
      <td>6460</td>
    </tr>
    <tr>
      <th>606</th>
      <td>Straight Outta Compton</td>
      <td>2015</td>
      <td>R</td>
      <td>147</td>
      <td>Biography, Drama, History</td>
      <td>7.8</td>
      <td>The rap group NWA emerges from the mean street...</td>
      <td>72.00000</td>
      <td>F. Gary Gray</td>
      <td>O'Shea Jackson Jr.</td>
      <td>Corey Hawkins</td>
      <td>Jason Mitchell</td>
      <td>Neil Brown Jr.</td>
      <td>179264</td>
      <td>161197785</td>
    </tr>
    <tr>
      <th>607</th>
      <td>Madeo</td>
      <td>2009</td>
      <td>R</td>
      <td>129</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.8</td>
      <td>A mother desperately searches for the killer w...</td>
      <td>79.00000</td>
      <td>Bong Joon Ho</td>
      <td>Hye-ja Kim</td>
      <td>Won Bin</td>
      <td>Jin Goo</td>
      <td>Je-mun Yun</td>
      <td>52758</td>
      <td>547292</td>
    </tr>
    <tr>
      <th>608</th>
      <td>Chugyeokja</td>
      <td>2008</td>
      <td>Unknown</td>
      <td>125</td>
      <td>Action, Crime, Thriller</td>
      <td>7.8</td>
      <td>A disgraced ex-policeman who runs a small ring...</td>
      <td>64.00000</td>
      <td>Hong-jin Na</td>
      <td>Kim Yoon-seok</td>
      <td>Jung-woo Ha</td>
      <td>Yeong-hie Seo</td>
      <td>Yoo-Jeong Kim</td>
      <td>58468</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>609</th>
      <td>The Hobbit: The Desolation of Smaug</td>
      <td>2013</td>
      <td>UA</td>
      <td>161</td>
      <td>Adventure, Fantasy</td>
      <td>7.8</td>
      <td>The dwarves, along with Bilbo Baggins and Gand...</td>
      <td>66.00000</td>
      <td>Peter Jackson</td>
      <td>Ian McKellen</td>
      <td>Martin Freeman</td>
      <td>Richard Armitage</td>
      <td>Ken Stott</td>
      <td>601408</td>
      <td>258366855</td>
    </tr>
    <tr>
      <th>610</th>
      <td>Das weiße Band - Eine deutsche Kindergeschichte</td>
      <td>2009</td>
      <td>UA</td>
      <td>144</td>
      <td>Drama, History, Mystery</td>
      <td>7.8</td>
      <td>Strange events happen in a small village in th...</td>
      <td>82.00000</td>
      <td>Michael Haneke</td>
      <td>Christian Friedel</td>
      <td>Ernst Jacobi</td>
      <td>Leonie Benesch</td>
      <td>Ulrich Tukur</td>
      <td>68715</td>
      <td>2222647</td>
    </tr>
    <tr>
      <th>611</th>
      <td>Män som hatar kvinnor</td>
      <td>2009</td>
      <td>R</td>
      <td>152</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.8</td>
      <td>A journalist is aided by a young female hacker...</td>
      <td>76.00000</td>
      <td>Niels Arden Oplev</td>
      <td>Michael Nyqvist</td>
      <td>Noomi Rapace</td>
      <td>Ewa Fröling</td>
      <td>Lena Endre</td>
      <td>208994</td>
      <td>10095170</td>
    </tr>
    <tr>
      <th>612</th>
      <td>The Trial of the Chicago 7</td>
      <td>2020</td>
      <td>R</td>
      <td>129</td>
      <td>Drama, History, Thriller</td>
      <td>7.8</td>
      <td>The story of 7 people on trial stemming from v...</td>
      <td>77.00000</td>
      <td>Aaron Sorkin</td>
      <td>Eddie Redmayne</td>
      <td>Alex Sharp</td>
      <td>Sacha Baron Cohen</td>
      <td>Jeremy Strong</td>
      <td>89896</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>613</th>
      <td>Druk</td>
      <td>2020</td>
      <td>Unknown</td>
      <td>117</td>
      <td>Comedy, Drama</td>
      <td>7.8</td>
      <td>Four friends, all high school teachers, test a...</td>
      <td>81.00000</td>
      <td>Thomas Vinterberg</td>
      <td>Mads Mikkelsen</td>
      <td>Thomas Bo Larsen</td>
      <td>Magnus Millang</td>
      <td>Lars Ranthe</td>
      <td>33931</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>614</th>
      <td>The Fighter</td>
      <td>2010</td>
      <td>UA</td>
      <td>116</td>
      <td>Biography, Drama, Sport</td>
      <td>7.8</td>
      <td>Based on the story of Micky Ward, a fledgling ...</td>
      <td>79.00000</td>
      <td>David O. Russell</td>
      <td>Mark Wahlberg</td>
      <td>Christian Bale</td>
      <td>Amy Adams</td>
      <td>Melissa Leo</td>
      <td>340584</td>
      <td>93617009</td>
    </tr>
    <tr>
      <th>615</th>
      <td>Taken</td>
      <td>2008</td>
      <td>A</td>
      <td>90</td>
      <td>Action, Thriller</td>
      <td>7.8</td>
      <td>A retired CIA agent travels across Europe and ...</td>
      <td>51.00000</td>
      <td>Pierre Morel</td>
      <td>Liam Neeson</td>
      <td>Maggie Grace</td>
      <td>Famke Janssen</td>
      <td>Leland Orser</td>
      <td>564791</td>
      <td>145000989</td>
    </tr>
    <tr>
      <th>616</th>
      <td>The Boy in the Striped Pyjamas</td>
      <td>2008</td>
      <td>PG-13</td>
      <td>94</td>
      <td>Drama, History, War</td>
      <td>7.8</td>
      <td>Through the innocent eyes of Bruno, the eight-...</td>
      <td>55.00000</td>
      <td>Mark Herman</td>
      <td>Asa Butterfield</td>
      <td>David Thewlis</td>
      <td>Rupert Friend</td>
      <td>Zac Mattoon O'Brien</td>
      <td>190748</td>
      <td>9030581</td>
    </tr>
    <tr>
      <th>617</th>
      <td>Once</td>
      <td>2007</td>
      <td>R</td>
      <td>86</td>
      <td>Drama, Music, Romance</td>
      <td>7.8</td>
      <td>A modern-day musical about a busker and an imm...</td>
      <td>88.00000</td>
      <td>John Carney</td>
      <td>Glen Hansard</td>
      <td>Markéta Irglová</td>
      <td>Hugh Walsh</td>
      <td>Gerard Hendrick</td>
      <td>110656</td>
      <td>9439923</td>
    </tr>
    <tr>
      <th>618</th>
      <td>The Hobbit: An Unexpected Journey</td>
      <td>2012</td>
      <td>UA</td>
      <td>169</td>
      <td>Adventure, Fantasy</td>
      <td>7.8</td>
      <td>A reluctant Hobbit, Bilbo Baggins, sets out to...</td>
      <td>58.00000</td>
      <td>Peter Jackson</td>
      <td>Martin Freeman</td>
      <td>Ian McKellen</td>
      <td>Richard Armitage</td>
      <td>Andy Serkis</td>
      <td>757377</td>
      <td>303003568</td>
    </tr>
    <tr>
      <th>619</th>
      <td>Auf der anderen Seite</td>
      <td>2007</td>
      <td>Unknown</td>
      <td>122</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>A Turkish man travels to Istanbul to find the ...</td>
      <td>85.00000</td>
      <td>Fatih Akin</td>
      <td>Baki Davrak</td>
      <td>Nurgül Yesilçay</td>
      <td>Tuncel Kurtiz</td>
      <td>Nursel Köse</td>
      <td>30827</td>
      <td>741283</td>
    </tr>
    <tr>
      <th>620</th>
      <td>Atonement</td>
      <td>2007</td>
      <td>R</td>
      <td>123</td>
      <td>Drama, Mystery, Romance</td>
      <td>7.8</td>
      <td>Thirteen-year-old fledgling writer Briony Tall...</td>
      <td>85.00000</td>
      <td>Joe Wright</td>
      <td>Keira Knightley</td>
      <td>James McAvoy</td>
      <td>Brenda Blethyn</td>
      <td>Saoirse Ronan</td>
      <td>251370</td>
      <td>50927067</td>
    </tr>
    <tr>
      <th>621</th>
      <td>Drive</td>
      <td>2011</td>
      <td>A</td>
      <td>100</td>
      <td>Crime, Drama</td>
      <td>7.8</td>
      <td>A mysterious Hollywood stuntman and mechanic m...</td>
      <td>78.00000</td>
      <td>Nicolas Winding Refn</td>
      <td>Ryan Gosling</td>
      <td>Carey Mulligan</td>
      <td>Bryan Cranston</td>
      <td>Albert Brooks</td>
      <td>571571</td>
      <td>35061555</td>
    </tr>
    <tr>
      <th>622</th>
      <td>American Gangster</td>
      <td>2007</td>
      <td>A</td>
      <td>157</td>
      <td>Biography, Crime, Drama</td>
      <td>7.8</td>
      <td>An outcast New York City cop is charged with b...</td>
      <td>76.00000</td>
      <td>Ridley Scott</td>
      <td>Denzel Washington</td>
      <td>Russell Crowe</td>
      <td>Chiwetel Ejiofor</td>
      <td>Josh Brolin</td>
      <td>392449</td>
      <td>130164645</td>
    </tr>
    <tr>
      <th>623</th>
      <td>Avatar</td>
      <td>2009</td>
      <td>UA</td>
      <td>162</td>
      <td>Action, Adventure, Fantasy</td>
      <td>7.8</td>
      <td>A paraplegic Marine dispatched to the moon Pan...</td>
      <td>83.00000</td>
      <td>James Cameron</td>
      <td>Sam Worthington</td>
      <td>Zoe Saldana</td>
      <td>Sigourney Weaver</td>
      <td>Michelle Rodriguez</td>
      <td>1118998</td>
      <td>760507625</td>
    </tr>
    <tr>
      <th>624</th>
      <td>Mr. Nobody</td>
      <td>2009</td>
      <td>R</td>
      <td>141</td>
      <td>Drama, Fantasy, Romance</td>
      <td>7.8</td>
      <td>A boy stands on a station platform as a train ...</td>
      <td>63.00000</td>
      <td>Jaco Van Dormael</td>
      <td>Jared Leto</td>
      <td>Sarah Polley</td>
      <td>Diane Kruger</td>
      <td>Linh Dan Pham</td>
      <td>216421</td>
      <td>3600</td>
    </tr>
    <tr>
      <th>625</th>
      <td>Apocalypto</td>
      <td>2006</td>
      <td>A</td>
      <td>139</td>
      <td>Action, Adventure, Drama</td>
      <td>7.8</td>
      <td>As the Mayan kingdom faces its decline, a youn...</td>
      <td>68.00000</td>
      <td>Mel Gibson</td>
      <td>Gerardo Taracena</td>
      <td>Raoul Max Trujillo</td>
      <td>Dalia Hernández</td>
      <td>Rudy Youngblood</td>
      <td>291018</td>
      <td>50866635</td>
    </tr>
    <tr>
      <th>626</th>
      <td>Little Miss Sunshine</td>
      <td>2006</td>
      <td>UA</td>
      <td>101</td>
      <td>Comedy, Drama</td>
      <td>7.8</td>
      <td>A family determined to get their young daughte...</td>
      <td>80.00000</td>
      <td>Jonathan Dayton</td>
      <td>Valerie Faris</td>
      <td>Steve Carell</td>
      <td>Toni Collette</td>
      <td>Greg Kinnear</td>
      <td>439856</td>
      <td>59891098</td>
    </tr>
    <tr>
      <th>627</th>
      <td>Hot Fuzz</td>
      <td>2007</td>
      <td>UA</td>
      <td>121</td>
      <td>Action, Comedy, Mystery</td>
      <td>7.8</td>
      <td>A skilled London police officer is transferred...</td>
      <td>81.00000</td>
      <td>Edgar Wright</td>
      <td>Simon Pegg</td>
      <td>Nick Frost</td>
      <td>Martin Freeman</td>
      <td>Bill Nighy</td>
      <td>463466</td>
      <td>23637265</td>
    </tr>
    <tr>
      <th>628</th>
      <td>The Curious Case of Benjamin Button</td>
      <td>2008</td>
      <td>UA</td>
      <td>166</td>
      <td>Drama, Fantasy, Romance</td>
      <td>7.8</td>
      <td>Tells the story of Benjamin Button, a man who ...</td>
      <td>70.00000</td>
      <td>David Fincher</td>
      <td>Brad Pitt</td>
      <td>Cate Blanchett</td>
      <td>Tilda Swinton</td>
      <td>Julia Ormond</td>
      <td>589160</td>
      <td>127509326</td>
    </tr>
    <tr>
      <th>629</th>
      <td>Veer-Zaara</td>
      <td>2004</td>
      <td>U</td>
      <td>192</td>
      <td>Drama, Family, Musical</td>
      <td>7.8</td>
      <td>Veer-Zaara is a saga of love, separation, cour...</td>
      <td>67.00000</td>
      <td>Yash Chopra</td>
      <td>Shah Rukh Khan</td>
      <td>Preity Zinta</td>
      <td>Rani Mukerji</td>
      <td>Kirron Kher</td>
      <td>49050</td>
      <td>2921738</td>
    </tr>
    <tr>
      <th>630</th>
      <td>Adams æbler</td>
      <td>2005</td>
      <td>R</td>
      <td>94</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.8</td>
      <td>A neo-nazi sentenced to community service at a...</td>
      <td>51.00000</td>
      <td>Anders Thomas Jensen</td>
      <td>Ulrich Thomsen</td>
      <td>Mads Mikkelsen</td>
      <td>Nicolas Bro</td>
      <td>Paprika Steen</td>
      <td>45717</td>
      <td>1305</td>
    </tr>
    <tr>
      <th>631</th>
      <td>Pride &amp; Prejudice</td>
      <td>2005</td>
      <td>PG</td>
      <td>129</td>
      <td>Drama, Romance</td>
      <td>7.8</td>
      <td>Sparks fly when spirited Elizabeth Bennet meet...</td>
      <td>82.00000</td>
      <td>Joe Wright</td>
      <td>Keira Knightley</td>
      <td>Matthew Macfadyen</td>
      <td>Brenda Blethyn</td>
      <td>Donald Sutherland</td>
      <td>258924</td>
      <td>38405088</td>
    </tr>
    <tr>
      <th>632</th>
      <td>The World's Fastest Indian</td>
      <td>2005</td>
      <td>U</td>
      <td>127</td>
      <td>Biography, Drama, Sport</td>
      <td>7.8</td>
      <td>The story of New Zealander Burt Munro, who spe...</td>
      <td>68.00000</td>
      <td>Roger Donaldson</td>
      <td>Anthony Hopkins</td>
      <td>Diane Ladd</td>
      <td>Iain Rea</td>
      <td>Tessa Mitchell</td>
      <td>51980</td>
      <td>5128124</td>
    </tr>
    <tr>
      <th>633</th>
      <td>Tôkyô goddofâzâzu</td>
      <td>2003</td>
      <td>UA</td>
      <td>90</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.8</td>
      <td>On Christmas Eve, three homeless people living...</td>
      <td>73.00000</td>
      <td>Satoshi Kon</td>
      <td>Shôgo Furuya</td>
      <td>Tôru Emori</td>
      <td>Yoshiaki Umegaki</td>
      <td>Aya Okamoto</td>
      <td>31658</td>
      <td>128985</td>
    </tr>
    <tr>
      <th>634</th>
      <td>Serenity</td>
      <td>2005</td>
      <td>PG-13</td>
      <td>119</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.8</td>
      <td>The crew of the ship Serenity try to evade an ...</td>
      <td>74.00000</td>
      <td>Joss Whedon</td>
      <td>Nathan Fillion</td>
      <td>Gina Torres</td>
      <td>Chiwetel Ejiofor</td>
      <td>Alan Tudyk</td>
      <td>283310</td>
      <td>25514517</td>
    </tr>
    <tr>
      <th>635</th>
      <td>Walk the Line</td>
      <td>2005</td>
      <td>PG-13</td>
      <td>136</td>
      <td>Biography, Drama, Music</td>
      <td>7.8</td>
      <td>A chronicle of country music legend Johnny Cas...</td>
      <td>72.00000</td>
      <td>James Mangold</td>
      <td>Joaquin Phoenix</td>
      <td>Reese Witherspoon</td>
      <td>Ginnifer Goodwin</td>
      <td>Robert Patrick</td>
      <td>234207</td>
      <td>119519402</td>
    </tr>
    <tr>
      <th>636</th>
      <td>Ondskan</td>
      <td>2003</td>
      <td>Unknown</td>
      <td>113</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>A teenage boy expelled from school for fightin...</td>
      <td>61.00000</td>
      <td>Mikael Håfström</td>
      <td>Andreas Wilson</td>
      <td>Henrik Lundström</td>
      <td>Gustaf Skarsgård</td>
      <td>Linda Zilliacus</td>
      <td>35682</td>
      <td>15280</td>
    </tr>
    <tr>
      <th>637</th>
      <td>The Notebook</td>
      <td>2004</td>
      <td>A</td>
      <td>123</td>
      <td>Drama, Romance</td>
      <td>7.8</td>
      <td>A poor yet passionate young man falls in love ...</td>
      <td>53.00000</td>
      <td>Nick Cassavetes</td>
      <td>Gena Rowlands</td>
      <td>James Garner</td>
      <td>Rachel McAdams</td>
      <td>Ryan Gosling</td>
      <td>520284</td>
      <td>81001787</td>
    </tr>
    <tr>
      <th>638</th>
      <td>Diarios de motocicleta</td>
      <td>2004</td>
      <td>U</td>
      <td>126</td>
      <td>Adventure, Biography, Drama</td>
      <td>7.8</td>
      <td>The dramatization of a motorcycle road trip Ch...</td>
      <td>75.00000</td>
      <td>Walter Salles</td>
      <td>Gael García Bernal</td>
      <td>Rodrigo De la Serna</td>
      <td>Mía Maestro</td>
      <td>Mercedes Morán</td>
      <td>96703</td>
      <td>16756372</td>
    </tr>
    <tr>
      <th>639</th>
      <td>Lilja 4-ever</td>
      <td>2002</td>
      <td>R</td>
      <td>109</td>
      <td>Crime, Drama</td>
      <td>7.8</td>
      <td>Sixteen-year-old Lilja and her only friend, th...</td>
      <td>82.00000</td>
      <td>Lukas Moodysson</td>
      <td>Oksana Akinshina</td>
      <td>Artyom Bogucharskiy</td>
      <td>Pavel Ponomaryov</td>
      <td>Lyubov Agapova</td>
      <td>42673</td>
      <td>181655</td>
    </tr>
    <tr>
      <th>640</th>
      <td>Les triplettes de Belleville</td>
      <td>2003</td>
      <td>PG-13</td>
      <td>80</td>
      <td>Animation, Comedy, Drama</td>
      <td>7.8</td>
      <td>When her grandson is kidnapped during the Tour...</td>
      <td>91.00000</td>
      <td>Sylvain Chomet</td>
      <td>Michèle Caucheteux</td>
      <td>Jean-Claude Donda</td>
      <td>Michel Robin</td>
      <td>Monica Viegas</td>
      <td>50622</td>
      <td>7002255</td>
    </tr>
    <tr>
      <th>641</th>
      <td>Gongdong gyeongbi guyeok JSA</td>
      <td>2000</td>
      <td>Unknown</td>
      <td>110</td>
      <td>Action, Drama, Thriller</td>
      <td>7.8</td>
      <td>After a shooting incident at the North/South K...</td>
      <td>58.00000</td>
      <td>Chan-wook Park</td>
      <td>Lee Yeong-ae</td>
      <td>Lee Byung-Hun</td>
      <td>Kang-ho Song</td>
      <td>Kim Tae-Woo</td>
      <td>26518</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>642</th>
      <td>The Count of Monte Cristo</td>
      <td>2002</td>
      <td>PG-13</td>
      <td>131</td>
      <td>Action, Adventure, Drama</td>
      <td>7.8</td>
      <td>A young man, falsely imprisoned by his jealous...</td>
      <td>61.00000</td>
      <td>Kevin Reynolds</td>
      <td>Jim Caviezel</td>
      <td>Guy Pearce</td>
      <td>Christopher Adamson</td>
      <td>JB Blanc</td>
      <td>129022</td>
      <td>54234062</td>
    </tr>
    <tr>
      <th>643</th>
      <td>Waking Life</td>
      <td>2001</td>
      <td>R</td>
      <td>99</td>
      <td>Animation, Drama, Fantasy</td>
      <td>7.8</td>
      <td>A man shuffles through a dream meeting various...</td>
      <td>83.00000</td>
      <td>Richard Linklater</td>
      <td>Ethan Hawke</td>
      <td>Trevor Jack Brooks</td>
      <td>Lorelei Linklater</td>
      <td>Wiley Wiggins</td>
      <td>60684</td>
      <td>2892011</td>
    </tr>
    <tr>
      <th>644</th>
      <td>Remember the Titans</td>
      <td>2000</td>
      <td>U</td>
      <td>113</td>
      <td>Biography, Drama, Sport</td>
      <td>7.8</td>
      <td>The true story of a newly appointed African-Am...</td>
      <td>48.00000</td>
      <td>Boaz Yakin</td>
      <td>Denzel Washington</td>
      <td>Will Patton</td>
      <td>Wood Harris</td>
      <td>Ryan Hurst</td>
      <td>198089</td>
      <td>115654751</td>
    </tr>
    <tr>
      <th>645</th>
      <td>Wo hu cang long</td>
      <td>2000</td>
      <td>UA</td>
      <td>120</td>
      <td>Action, Adventure, Fantasy</td>
      <td>7.8</td>
      <td>A young Chinese warrior steals a sword from a ...</td>
      <td>94.00000</td>
      <td>Ang Lee</td>
      <td>Yun-Fat Chow</td>
      <td>Michelle Yeoh</td>
      <td>Ziyi Zhang</td>
      <td>Chen Chang</td>
      <td>253228</td>
      <td>128078872</td>
    </tr>
    <tr>
      <th>646</th>
      <td>Todo sobre mi madre</td>
      <td>1999</td>
      <td>R</td>
      <td>101</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>Young Esteban wants to become a writer and als...</td>
      <td>87.00000</td>
      <td>Pedro Almodóvar</td>
      <td>Cecilia Roth</td>
      <td>Marisa Paredes</td>
      <td>Candela Peña</td>
      <td>Antonia San Juan</td>
      <td>89058</td>
      <td>8264530</td>
    </tr>
    <tr>
      <th>647</th>
      <td>Cast Away</td>
      <td>2000</td>
      <td>UA</td>
      <td>143</td>
      <td>Adventure, Drama, Romance</td>
      <td>7.8</td>
      <td>A FedEx executive undergoes a physical and emo...</td>
      <td>73.00000</td>
      <td>Robert Zemeckis</td>
      <td>Tom Hanks</td>
      <td>Helen Hunt</td>
      <td>Paul Sanchez</td>
      <td>Lari White</td>
      <td>524235</td>
      <td>233632142</td>
    </tr>
    <tr>
      <th>648</th>
      <td>The Boondock Saints</td>
      <td>1999</td>
      <td>R</td>
      <td>108</td>
      <td>Action, Crime, Thriller</td>
      <td>7.8</td>
      <td>Two Irish Catholic brothers become vigilantes ...</td>
      <td>44.00000</td>
      <td>Troy Duffy</td>
      <td>Willem Dafoe</td>
      <td>Sean Patrick Flanery</td>
      <td>Norman Reedus</td>
      <td>David Della Rocco</td>
      <td>227143</td>
      <td>25812</td>
    </tr>
    <tr>
      <th>649</th>
      <td>The Insider</td>
      <td>1999</td>
      <td>UA</td>
      <td>157</td>
      <td>Biography, Drama, Thriller</td>
      <td>7.8</td>
      <td>A research chemist comes under personal and pr...</td>
      <td>84.00000</td>
      <td>Michael Mann</td>
      <td>Russell Crowe</td>
      <td>Al Pacino</td>
      <td>Christopher Plummer</td>
      <td>Diane Venora</td>
      <td>159886</td>
      <td>28965197</td>
    </tr>
    <tr>
      <th>650</th>
      <td>October Sky</td>
      <td>1999</td>
      <td>PG</td>
      <td>108</td>
      <td>Biography, Drama, Family</td>
      <td>7.8</td>
      <td>The true story of Homer Hickam, a coal miner's...</td>
      <td>71.00000</td>
      <td>Joe Johnston</td>
      <td>Jake Gyllenhaal</td>
      <td>Chris Cooper</td>
      <td>Laura Dern</td>
      <td>Chris Owen</td>
      <td>82855</td>
      <td>32481825</td>
    </tr>
    <tr>
      <th>651</th>
      <td>Shrek</td>
      <td>2001</td>
      <td>U</td>
      <td>90</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.8</td>
      <td>A mean lord exiles fairytale creatures to the ...</td>
      <td>84.00000</td>
      <td>Andrew Adamson</td>
      <td>Vicky Jenson</td>
      <td>Mike Myers</td>
      <td>Eddie Murphy</td>
      <td>Cameron Diaz</td>
      <td>613941</td>
      <td>267665011</td>
    </tr>
    <tr>
      <th>652</th>
      <td>Titanic</td>
      <td>1997</td>
      <td>UA</td>
      <td>194</td>
      <td>Drama, Romance</td>
      <td>7.8</td>
      <td>A seventeen-year-old aristocrat falls in love ...</td>
      <td>75.00000</td>
      <td>James Cameron</td>
      <td>Leonardo DiCaprio</td>
      <td>Kate Winslet</td>
      <td>Billy Zane</td>
      <td>Kathy Bates</td>
      <td>1046089</td>
      <td>659325379</td>
    </tr>
    <tr>
      <th>653</th>
      <td>Hana-bi</td>
      <td>1997</td>
      <td>Unknown</td>
      <td>103</td>
      <td>Crime, Drama, Romance</td>
      <td>7.8</td>
      <td>Nishi leaves the police in the face of harrowi...</td>
      <td>77.97153</td>
      <td>Takeshi Kitano</td>
      <td>Takeshi Kitano</td>
      <td>Kayoko Kishimoto</td>
      <td>Ren Osugi</td>
      <td>Susumu Terajima</td>
      <td>27712</td>
      <td>233986</td>
    </tr>
    <tr>
      <th>654</th>
      <td>Gattaca</td>
      <td>1997</td>
      <td>UA</td>
      <td>106</td>
      <td>Drama, Sci-Fi, Thriller</td>
      <td>7.8</td>
      <td>A genetically inferior man assumes the identit...</td>
      <td>64.00000</td>
      <td>Andrew Niccol</td>
      <td>Ethan Hawke</td>
      <td>Uma Thurman</td>
      <td>Jude Law</td>
      <td>Gore Vidal</td>
      <td>280845</td>
      <td>12339633</td>
    </tr>
    <tr>
      <th>655</th>
      <td>The Game</td>
      <td>1997</td>
      <td>UA</td>
      <td>129</td>
      <td>Action, Drama, Mystery</td>
      <td>7.8</td>
      <td>After a wealthy banker is given an opportunity...</td>
      <td>61.00000</td>
      <td>David Fincher</td>
      <td>Michael Douglas</td>
      <td>Deborah Kara Unger</td>
      <td>Sean Penn</td>
      <td>James Rebhorn</td>
      <td>345096</td>
      <td>48323648</td>
    </tr>
    <tr>
      <th>656</th>
      <td>Breaking the Waves</td>
      <td>1996</td>
      <td>R</td>
      <td>159</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>Oilman Jan is paralyzed in an accident. His wi...</td>
      <td>76.00000</td>
      <td>Lars von Trier</td>
      <td>Emily Watson</td>
      <td>Stellan Skarsgård</td>
      <td>Katrin Cartlidge</td>
      <td>Jean-Marc Barr</td>
      <td>62428</td>
      <td>4040691</td>
    </tr>
    <tr>
      <th>657</th>
      <td>Ed Wood</td>
      <td>1994</td>
      <td>U</td>
      <td>127</td>
      <td>Biography, Comedy, Drama</td>
      <td>7.8</td>
      <td>Ambitious but troubled movie director Edward D...</td>
      <td>70.00000</td>
      <td>Tim Burton</td>
      <td>Johnny Depp</td>
      <td>Martin Landau</td>
      <td>Sarah Jessica Parker</td>
      <td>Patricia Arquette</td>
      <td>164937</td>
      <td>5887457</td>
    </tr>
    <tr>
      <th>658</th>
      <td>What's Eating Gilbert Grape</td>
      <td>1993</td>
      <td>U</td>
      <td>118</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>A young man in a small Midwestern town struggl...</td>
      <td>73.00000</td>
      <td>Lasse Hallström</td>
      <td>Johnny Depp</td>
      <td>Leonardo DiCaprio</td>
      <td>Juliette Lewis</td>
      <td>Mary Steenburgen</td>
      <td>215034</td>
      <td>9170214</td>
    </tr>
    <tr>
      <th>659</th>
      <td>Tombstone</td>
      <td>1993</td>
      <td>R</td>
      <td>130</td>
      <td>Action, Biography, Drama</td>
      <td>7.8</td>
      <td>A successful lawman's plans to retire anonymou...</td>
      <td>50.00000</td>
      <td>George P. Cosmatos</td>
      <td>Kevin Jarre</td>
      <td>Kurt Russell</td>
      <td>Val Kilmer</td>
      <td>Sam Elliott</td>
      <td>126871</td>
      <td>56505065</td>
    </tr>
    <tr>
      <th>660</th>
      <td>The Sandlot</td>
      <td>1993</td>
      <td>U</td>
      <td>101</td>
      <td>Comedy, Drama, Family</td>
      <td>7.8</td>
      <td>In the summer of 1962, a new kid in town is ta...</td>
      <td>55.00000</td>
      <td>David Mickey Evans</td>
      <td>Tom Guiry</td>
      <td>Mike Vitar</td>
      <td>Art LaFleur</td>
      <td>Patrick Renna</td>
      <td>78963</td>
      <td>32416586</td>
    </tr>
    <tr>
      <th>661</th>
      <td>The Remains of the Day</td>
      <td>1993</td>
      <td>U</td>
      <td>134</td>
      <td>Drama, Romance</td>
      <td>7.8</td>
      <td>A butler who sacrificed body and soul to servi...</td>
      <td>84.00000</td>
      <td>James Ivory</td>
      <td>Anthony Hopkins</td>
      <td>Emma Thompson</td>
      <td>John Haycraft</td>
      <td>Christopher Reeve</td>
      <td>66065</td>
      <td>22954968</td>
    </tr>
    <tr>
      <th>662</th>
      <td>Naked</td>
      <td>1993</td>
      <td>Unknown</td>
      <td>132</td>
      <td>Comedy, Drama</td>
      <td>7.8</td>
      <td>Parallel tales of two sexually obsessed men, o...</td>
      <td>84.00000</td>
      <td>Mike Leigh</td>
      <td>David Thewlis</td>
      <td>Lesley Sharp</td>
      <td>Katrin Cartlidge</td>
      <td>Greg Cruttwell</td>
      <td>34635</td>
      <td>1769305</td>
    </tr>
    <tr>
      <th>663</th>
      <td>The Fugitive</td>
      <td>1993</td>
      <td>U</td>
      <td>130</td>
      <td>Action, Crime, Drama</td>
      <td>7.8</td>
      <td>Dr. Richard Kimble, unjustly accused of murder...</td>
      <td>87.00000</td>
      <td>Andrew Davis</td>
      <td>Harrison Ford</td>
      <td>Tommy Lee Jones</td>
      <td>Sela Ward</td>
      <td>Julianne Moore</td>
      <td>267684</td>
      <td>183875760</td>
    </tr>
    <tr>
      <th>664</th>
      <td>A Bronx Tale</td>
      <td>1993</td>
      <td>R</td>
      <td>121</td>
      <td>Crime, Drama, Romance</td>
      <td>7.8</td>
      <td>A father becomes worried when a local gangster...</td>
      <td>80.00000</td>
      <td>Robert De Niro</td>
      <td>Robert De Niro</td>
      <td>Chazz Palminteri</td>
      <td>Lillo Brancato</td>
      <td>Francis Capra</td>
      <td>128171</td>
      <td>17266971</td>
    </tr>
    <tr>
      <th>665</th>
      <td>Batman: Mask of the Phantasm</td>
      <td>1993</td>
      <td>PG</td>
      <td>76</td>
      <td>Animation, Action, Crime</td>
      <td>7.8</td>
      <td>Batman is wrongly implicated in a series of mu...</td>
      <td>77.97153</td>
      <td>Kevin Altieri</td>
      <td>Boyd Kirkland</td>
      <td>Frank Paur</td>
      <td>Dan Riba</td>
      <td>Eric Radomski</td>
      <td>43690</td>
      <td>5617391</td>
    </tr>
    <tr>
      <th>666</th>
      <td>Lat sau san taam</td>
      <td>1992</td>
      <td>R</td>
      <td>128</td>
      <td>Action, Crime, Thriller</td>
      <td>7.8</td>
      <td>A tough-as-nails cop teams up with an undercov...</td>
      <td>77.97153</td>
      <td>John Woo</td>
      <td>Yun-Fat Chow</td>
      <td>Tony Chiu-Wai Leung</td>
      <td>Teresa Mo</td>
      <td>Philip Chan</td>
      <td>46700</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>667</th>
      <td>Night on Earth</td>
      <td>1991</td>
      <td>R</td>
      <td>129</td>
      <td>Comedy, Drama</td>
      <td>7.8</td>
      <td>An anthology of 5 different cab drivers in 5 A...</td>
      <td>68.00000</td>
      <td>Jim Jarmusch</td>
      <td>Winona Ryder</td>
      <td>Gena Rowlands</td>
      <td>Lisanne Falk</td>
      <td>Alan Randolph Scott</td>
      <td>55362</td>
      <td>2015810</td>
    </tr>
    <tr>
      <th>668</th>
      <td>La double vie de Véronique</td>
      <td>1991</td>
      <td>R</td>
      <td>98</td>
      <td>Drama, Fantasy, Music</td>
      <td>7.8</td>
      <td>Two parallel stories about two identical women...</td>
      <td>86.00000</td>
      <td>Krzysztof Kieslowski</td>
      <td>Irène Jacob</td>
      <td>Wladyslaw Kowalski</td>
      <td>Halina Gryglaszewska</td>
      <td>Kalina Jedrusik</td>
      <td>42376</td>
      <td>1999955</td>
    </tr>
    <tr>
      <th>669</th>
      <td>Boyz n the Hood</td>
      <td>1991</td>
      <td>A</td>
      <td>112</td>
      <td>Crime, Drama</td>
      <td>7.8</td>
      <td>Follows the lives of three young males living ...</td>
      <td>76.00000</td>
      <td>John Singleton</td>
      <td>Cuba Gooding Jr.</td>
      <td>Laurence Fishburne</td>
      <td>Hudhail Al-Amir</td>
      <td>Lloyd Avery II</td>
      <td>126082</td>
      <td>57504069</td>
    </tr>
    <tr>
      <th>670</th>
      <td>Misery</td>
      <td>1990</td>
      <td>R</td>
      <td>107</td>
      <td>Drama, Thriller</td>
      <td>7.8</td>
      <td>After a famous author is rescued from a car cr...</td>
      <td>75.00000</td>
      <td>Rob Reiner</td>
      <td>James Caan</td>
      <td>Kathy Bates</td>
      <td>Richard Farnsworth</td>
      <td>Frances Sternhagen</td>
      <td>184740</td>
      <td>61276872</td>
    </tr>
    <tr>
      <th>671</th>
      <td>Awakenings</td>
      <td>1990</td>
      <td>U</td>
      <td>121</td>
      <td>Biography, Drama</td>
      <td>7.8</td>
      <td>The victims of an encephalitis epidemic many y...</td>
      <td>74.00000</td>
      <td>Penny Marshall</td>
      <td>Robert De Niro</td>
      <td>Robin Williams</td>
      <td>Julie Kavner</td>
      <td>Ruth Nelson</td>
      <td>125276</td>
      <td>52096475</td>
    </tr>
    <tr>
      <th>672</th>
      <td>Majo no takkyûbin</td>
      <td>1989</td>
      <td>U</td>
      <td>103</td>
      <td>Animation, Adventure, Drama</td>
      <td>7.8</td>
      <td>A young witch, on her mandatory year of indepe...</td>
      <td>83.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Kirsten Dunst</td>
      <td>Minami Takayama</td>
      <td>Rei Sakuma</td>
      <td>Kappei Yamaguchi</td>
      <td>124193</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>673</th>
      <td>Glory</td>
      <td>1989</td>
      <td>R</td>
      <td>122</td>
      <td>Biography, Drama, History</td>
      <td>7.8</td>
      <td>Robert Gould Shaw leads the U.S. Civil War's f...</td>
      <td>78.00000</td>
      <td>Edward Zwick</td>
      <td>Matthew Broderick</td>
      <td>Denzel Washington</td>
      <td>Cary Elwes</td>
      <td>Morgan Freeman</td>
      <td>122779</td>
      <td>26830000</td>
    </tr>
    <tr>
      <th>674</th>
      <td>Dip huet seung hung</td>
      <td>1989</td>
      <td>R</td>
      <td>111</td>
      <td>Action, Crime, Drama</td>
      <td>7.8</td>
      <td>A disillusioned assassin accepts one last hit ...</td>
      <td>82.00000</td>
      <td>John Woo</td>
      <td>Yun-Fat Chow</td>
      <td>Danny Lee</td>
      <td>Sally Yeh</td>
      <td>Kong Chu</td>
      <td>45624</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>675</th>
      <td>Back to the Future Part II</td>
      <td>1989</td>
      <td>U</td>
      <td>108</td>
      <td>Adventure, Comedy, Sci-Fi</td>
      <td>7.8</td>
      <td>After visiting 2015, Marty McFly must repeat h...</td>
      <td>57.00000</td>
      <td>Robert Zemeckis</td>
      <td>Michael J. Fox</td>
      <td>Christopher Lloyd</td>
      <td>Lea Thompson</td>
      <td>Thomas F. Wilson</td>
      <td>481918</td>
      <td>118500000</td>
    </tr>
    <tr>
      <th>676</th>
      <td>Mississippi Burning</td>
      <td>1988</td>
      <td>A</td>
      <td>128</td>
      <td>Crime, Drama, History</td>
      <td>7.8</td>
      <td>Two F.B.I. Agents with wildly different styles...</td>
      <td>65.00000</td>
      <td>Alan Parker</td>
      <td>Gene Hackman</td>
      <td>Willem Dafoe</td>
      <td>Frances McDormand</td>
      <td>Brad Dourif</td>
      <td>88214</td>
      <td>34603943</td>
    </tr>
    <tr>
      <th>677</th>
      <td>Predator</td>
      <td>1987</td>
      <td>A</td>
      <td>107</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.8</td>
      <td>A team of commandos on a mission in a Central ...</td>
      <td>45.00000</td>
      <td>John McTiernan</td>
      <td>Arnold Schwarzenegger</td>
      <td>Carl Weathers</td>
      <td>Kevin Peter Hall</td>
      <td>Elpidia Carrillo</td>
      <td>371387</td>
      <td>59735548</td>
    </tr>
    <tr>
      <th>678</th>
      <td>Evil Dead II</td>
      <td>1987</td>
      <td>A</td>
      <td>84</td>
      <td>Action, Comedy, Fantasy</td>
      <td>7.8</td>
      <td>The lone survivor of an onslaught of flesh-pos...</td>
      <td>72.00000</td>
      <td>Sam Raimi</td>
      <td>Bruce Campbell</td>
      <td>Sarah Berry</td>
      <td>Dan Hicks</td>
      <td>Kassie Wesley DePaiva</td>
      <td>148359</td>
      <td>5923044</td>
    </tr>
    <tr>
      <th>679</th>
      <td>Ferris Bueller's Day Off</td>
      <td>1986</td>
      <td>U</td>
      <td>103</td>
      <td>Comedy</td>
      <td>7.8</td>
      <td>A high school wise guy is determined to have a...</td>
      <td>61.00000</td>
      <td>John Hughes</td>
      <td>Matthew Broderick</td>
      <td>Alan Ruck</td>
      <td>Mia Sara</td>
      <td>Jeffrey Jones</td>
      <td>321382</td>
      <td>70136369</td>
    </tr>
    <tr>
      <th>680</th>
      <td>Down by Law</td>
      <td>1986</td>
      <td>R</td>
      <td>107</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.8</td>
      <td>Two men are framed and sent to jail, where the...</td>
      <td>75.00000</td>
      <td>Jim Jarmusch</td>
      <td>Tom Waits</td>
      <td>John Lurie</td>
      <td>Roberto Benigni</td>
      <td>Nicoletta Braschi</td>
      <td>47834</td>
      <td>1436000</td>
    </tr>
    <tr>
      <th>681</th>
      <td>The Goonies</td>
      <td>1985</td>
      <td>U</td>
      <td>114</td>
      <td>Adventure, Comedy, Family</td>
      <td>7.8</td>
      <td>A group of young misfits called The Goonies di...</td>
      <td>62.00000</td>
      <td>Richard Donner</td>
      <td>Sean Astin</td>
      <td>Josh Brolin</td>
      <td>Jeff Cohen</td>
      <td>Corey Feldman</td>
      <td>244430</td>
      <td>61503218</td>
    </tr>
    <tr>
      <th>682</th>
      <td>The Color Purple</td>
      <td>1985</td>
      <td>U</td>
      <td>154</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>A black Southern woman struggles to find her i...</td>
      <td>78.00000</td>
      <td>Steven Spielberg</td>
      <td>Danny Glover</td>
      <td>Whoopi Goldberg</td>
      <td>Oprah Winfrey</td>
      <td>Margaret Avery</td>
      <td>78321</td>
      <td>98467863</td>
    </tr>
    <tr>
      <th>683</th>
      <td>The Breakfast Club</td>
      <td>1985</td>
      <td>UA</td>
      <td>97</td>
      <td>Comedy, Drama</td>
      <td>7.8</td>
      <td>Five high school students meet in Saturday det...</td>
      <td>66.00000</td>
      <td>John Hughes</td>
      <td>Emilio Estevez</td>
      <td>Judd Nelson</td>
      <td>Molly Ringwald</td>
      <td>Ally Sheedy</td>
      <td>357026</td>
      <td>45875171</td>
    </tr>
    <tr>
      <th>684</th>
      <td>The Killing Fields</td>
      <td>1984</td>
      <td>UA</td>
      <td>141</td>
      <td>Biography, Drama, History</td>
      <td>7.8</td>
      <td>A journalist is trapped in Cambodia during tyr...</td>
      <td>76.00000</td>
      <td>Roland Joffé</td>
      <td>Sam Waterston</td>
      <td>Haing S. Ngor</td>
      <td>John Malkovich</td>
      <td>Julian Sands</td>
      <td>51585</td>
      <td>34700291</td>
    </tr>
    <tr>
      <th>685</th>
      <td>Ghostbusters</td>
      <td>1984</td>
      <td>UA</td>
      <td>105</td>
      <td>Action, Comedy, Fantasy</td>
      <td>7.8</td>
      <td>Three former parapsychology professors set up ...</td>
      <td>71.00000</td>
      <td>Ivan Reitman</td>
      <td>Bill Murray</td>
      <td>Dan Aykroyd</td>
      <td>Sigourney Weaver</td>
      <td>Harold Ramis</td>
      <td>355413</td>
      <td>238632124</td>
    </tr>
    <tr>
      <th>686</th>
      <td>The Right Stuff</td>
      <td>1983</td>
      <td>PG</td>
      <td>193</td>
      <td>Adventure, Biography, Drama</td>
      <td>7.8</td>
      <td>The story of the original Mercury 7 astronauts...</td>
      <td>91.00000</td>
      <td>Philip Kaufman</td>
      <td>Sam Shepard</td>
      <td>Scott Glenn</td>
      <td>Ed Harris</td>
      <td>Dennis Quaid</td>
      <td>56235</td>
      <td>21500000</td>
    </tr>
    <tr>
      <th>687</th>
      <td>The King of Comedy</td>
      <td>1982</td>
      <td>U</td>
      <td>109</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.8</td>
      <td>Rupert Pupkin is a passionate yet unsuccessful...</td>
      <td>73.00000</td>
      <td>Martin Scorsese</td>
      <td>Robert De Niro</td>
      <td>Jerry Lewis</td>
      <td>Diahnne Abbott</td>
      <td>Sandra Bernhard</td>
      <td>88511</td>
      <td>2500000</td>
    </tr>
    <tr>
      <th>688</th>
      <td>E.T. the Extra-Terrestrial</td>
      <td>1982</td>
      <td>U</td>
      <td>115</td>
      <td>Family, Sci-Fi</td>
      <td>7.8</td>
      <td>A troubled child summons the courage to help a...</td>
      <td>91.00000</td>
      <td>Steven Spielberg</td>
      <td>Henry Thomas</td>
      <td>Drew Barrymore</td>
      <td>Peter Coyote</td>
      <td>Dee Wallace</td>
      <td>372490</td>
      <td>435110554</td>
    </tr>
    <tr>
      <th>689</th>
      <td>Kramer vs. Kramer</td>
      <td>1979</td>
      <td>A</td>
      <td>105</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>Ted Kramer's wife leaves him, allowing for a l...</td>
      <td>77.00000</td>
      <td>Robert Benton</td>
      <td>Dustin Hoffman</td>
      <td>Meryl Streep</td>
      <td>Jane Alexander</td>
      <td>Justin Henry</td>
      <td>133351</td>
      <td>106260000</td>
    </tr>
    <tr>
      <th>690</th>
      <td>Days of Heaven</td>
      <td>1978</td>
      <td>PG</td>
      <td>94</td>
      <td>Drama, Romance</td>
      <td>7.8</td>
      <td>A hot-tempered farm laborer convinces the woma...</td>
      <td>93.00000</td>
      <td>Terrence Malick</td>
      <td>Richard Gere</td>
      <td>Brooke Adams</td>
      <td>Sam Shepard</td>
      <td>Linda Manz</td>
      <td>52852</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>691</th>
      <td>The Outlaw Josey Wales</td>
      <td>1976</td>
      <td>A</td>
      <td>135</td>
      <td>Western</td>
      <td>7.8</td>
      <td>Missouri farmer Josey Wales joins a Confederat...</td>
      <td>69.00000</td>
      <td>Clint Eastwood</td>
      <td>Clint Eastwood</td>
      <td>Sondra Locke</td>
      <td>Chief Dan George</td>
      <td>Bill McKinney</td>
      <td>65659</td>
      <td>31800000</td>
    </tr>
    <tr>
      <th>692</th>
      <td>The Man Who Would Be King</td>
      <td>1975</td>
      <td>PG</td>
      <td>129</td>
      <td>Adventure, History, War</td>
      <td>7.8</td>
      <td>Two British former soldiers decide to set them...</td>
      <td>91.00000</td>
      <td>John Huston</td>
      <td>Sean Connery</td>
      <td>Michael Caine</td>
      <td>Christopher Plummer</td>
      <td>Saeed Jaffrey</td>
      <td>44917</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>693</th>
      <td>The Conversation</td>
      <td>1974</td>
      <td>U</td>
      <td>113</td>
      <td>Drama, Mystery, Thriller</td>
      <td>7.8</td>
      <td>A paranoid, secretive surveillance expert has ...</td>
      <td>85.00000</td>
      <td>Francis Ford Coppola</td>
      <td>Gene Hackman</td>
      <td>John Cazale</td>
      <td>Allen Garfield</td>
      <td>Frederic Forrest</td>
      <td>98611</td>
      <td>4420000</td>
    </tr>
    <tr>
      <th>694</th>
      <td>La planète sauvage</td>
      <td>1973</td>
      <td>U</td>
      <td>72</td>
      <td>Animation, Sci-Fi</td>
      <td>7.8</td>
      <td>On a faraway planet where blue giants rule, op...</td>
      <td>73.00000</td>
      <td>René Laloux</td>
      <td>Barry Bostwick</td>
      <td>Jennifer Drake</td>
      <td>Eric Baugin</td>
      <td>Jean Topart</td>
      <td>25229</td>
      <td>193817</td>
    </tr>
    <tr>
      <th>695</th>
      <td>The Day of the Jackal</td>
      <td>1973</td>
      <td>A</td>
      <td>143</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.8</td>
      <td>A professional assassin codenamed "Jackal" plo...</td>
      <td>80.00000</td>
      <td>Fred Zinnemann</td>
      <td>Edward Fox</td>
      <td>Terence Alexander</td>
      <td>Michel Auclair</td>
      <td>Alan Badel</td>
      <td>37445</td>
      <td>16056255</td>
    </tr>
    <tr>
      <th>696</th>
      <td>Badlands</td>
      <td>1973</td>
      <td>PG</td>
      <td>94</td>
      <td>Action, Crime, Drama</td>
      <td>7.8</td>
      <td>An impressionable teenage girl from a dead-end...</td>
      <td>93.00000</td>
      <td>Terrence Malick</td>
      <td>Martin Sheen</td>
      <td>Sissy Spacek</td>
      <td>Warren Oates</td>
      <td>Ramon Bieri</td>
      <td>66009</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>697</th>
      <td>Cabaret</td>
      <td>1972</td>
      <td>A</td>
      <td>124</td>
      <td>Drama, Music, Musical</td>
      <td>7.8</td>
      <td>A female girlie club entertainer in Weimar Rep...</td>
      <td>80.00000</td>
      <td>Bob Fosse</td>
      <td>Liza Minnelli</td>
      <td>Michael York</td>
      <td>Helmut Griem</td>
      <td>Joel Grey</td>
      <td>48334</td>
      <td>42765000</td>
    </tr>
    <tr>
      <th>698</th>
      <td>Willy Wonka &amp; the Chocolate Factory</td>
      <td>1971</td>
      <td>U</td>
      <td>100</td>
      <td>Family, Fantasy, Musical</td>
      <td>7.8</td>
      <td>A poor but hopeful boy seeks one of the five c...</td>
      <td>67.00000</td>
      <td>Mel Stuart</td>
      <td>Gene Wilder</td>
      <td>Jack Albertson</td>
      <td>Peter Ostrum</td>
      <td>Roy Kinnear</td>
      <td>178731</td>
      <td>4000000</td>
    </tr>
    <tr>
      <th>699</th>
      <td>Midnight Cowboy</td>
      <td>1969</td>
      <td>A</td>
      <td>113</td>
      <td>Drama</td>
      <td>7.8</td>
      <td>A naive hustler travels from Texas to New York...</td>
      <td>79.00000</td>
      <td>John Schlesinger</td>
      <td>Dustin Hoffman</td>
      <td>Jon Voight</td>
      <td>Sylvia Miles</td>
      <td>John McGiver</td>
      <td>101124</td>
      <td>44785053</td>
    </tr>
    <tr>
      <th>700</th>
      <td>Wait Until Dark</td>
      <td>1967</td>
      <td>Unknown</td>
      <td>108</td>
      <td>Thriller</td>
      <td>7.8</td>
      <td>A recently blinded woman is terrorized by a tr...</td>
      <td>81.00000</td>
      <td>Terence Young</td>
      <td>Audrey Hepburn</td>
      <td>Alan Arkin</td>
      <td>Richard Crenna</td>
      <td>Efrem Zimbalist Jr.</td>
      <td>27733</td>
      <td>17550741</td>
    </tr>
    <tr>
      <th>701</th>
      <td>Guess Who's Coming to Dinner</td>
      <td>1967</td>
      <td>Unknown</td>
      <td>108</td>
      <td>Comedy, Drama</td>
      <td>7.8</td>
      <td>A couple's attitudes are challenged when their...</td>
      <td>63.00000</td>
      <td>Stanley Kramer</td>
      <td>Spencer Tracy</td>
      <td>Sidney Poitier</td>
      <td>Katharine Hepburn</td>
      <td>Katharine Houghton</td>
      <td>39642</td>
      <td>56700000</td>
    </tr>
    <tr>
      <th>702</th>
      <td>Bonnie and Clyde</td>
      <td>1967</td>
      <td>A</td>
      <td>111</td>
      <td>Action, Biography, Crime</td>
      <td>7.8</td>
      <td>Bored waitress Bonnie Parker falls in love wit...</td>
      <td>86.00000</td>
      <td>Arthur Penn</td>
      <td>Warren Beatty</td>
      <td>Faye Dunaway</td>
      <td>Michael J. Pollard</td>
      <td>Gene Hackman</td>
      <td>102415</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>703</th>
      <td>My Fair Lady</td>
      <td>1964</td>
      <td>U</td>
      <td>170</td>
      <td>Drama, Family, Musical</td>
      <td>7.8</td>
      <td>Snobbish phonetics Professor Henry Higgins agr...</td>
      <td>95.00000</td>
      <td>George Cukor</td>
      <td>Audrey Hepburn</td>
      <td>Rex Harrison</td>
      <td>Stanley Holloway</td>
      <td>Wilfrid Hyde-White</td>
      <td>86525</td>
      <td>72000000</td>
    </tr>
    <tr>
      <th>704</th>
      <td>Mary Poppins</td>
      <td>1964</td>
      <td>U</td>
      <td>139</td>
      <td>Comedy, Family, Fantasy</td>
      <td>7.8</td>
      <td>In turn of the century London, a magical nanny...</td>
      <td>88.00000</td>
      <td>Robert Stevenson</td>
      <td>Julie Andrews</td>
      <td>Dick Van Dyke</td>
      <td>David Tomlinson</td>
      <td>Glynis Johns</td>
      <td>158029</td>
      <td>102272727</td>
    </tr>
    <tr>
      <th>705</th>
      <td>The Longest Day</td>
      <td>1962</td>
      <td>G</td>
      <td>178</td>
      <td>Action, Drama, History</td>
      <td>7.8</td>
      <td>The events of D-Day, told on a grand scale fro...</td>
      <td>75.00000</td>
      <td>Ken Annakin</td>
      <td>Andrew Marton</td>
      <td>Gerd Oswald</td>
      <td>Bernhard Wicki</td>
      <td>Darryl F. Zanuck</td>
      <td>52141</td>
      <td>39100000</td>
    </tr>
    <tr>
      <th>706</th>
      <td>Jules et Jim</td>
      <td>1962</td>
      <td>Unknown</td>
      <td>105</td>
      <td>Drama, Romance</td>
      <td>7.8</td>
      <td>Decades of a love triangle concerning two frie...</td>
      <td>97.00000</td>
      <td>François Truffaut</td>
      <td>Jeanne Moreau</td>
      <td>Oskar Werner</td>
      <td>Henri Serre</td>
      <td>Vanna Urbino</td>
      <td>37605</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>707</th>
      <td>The Innocents</td>
      <td>1961</td>
      <td>A</td>
      <td>100</td>
      <td>Horror</td>
      <td>7.8</td>
      <td>A young governess for two children becomes con...</td>
      <td>88.00000</td>
      <td>Jack Clayton</td>
      <td>Deborah Kerr</td>
      <td>Peter Wyngarde</td>
      <td>Megs Jenkins</td>
      <td>Michael Redgrave</td>
      <td>27007</td>
      <td>2616000</td>
    </tr>
    <tr>
      <th>708</th>
      <td>À bout de souffle</td>
      <td>1960</td>
      <td>U</td>
      <td>90</td>
      <td>Crime, Drama</td>
      <td>7.8</td>
      <td>A small-time thief steals a car and impulsivel...</td>
      <td>77.97153</td>
      <td>Jean-Luc Godard</td>
      <td>Jean-Paul Belmondo</td>
      <td>Jean Seberg</td>
      <td>Daniel Boulanger</td>
      <td>Henri-Jacques Huet</td>
      <td>73251</td>
      <td>336705</td>
    </tr>
    <tr>
      <th>709</th>
      <td>Red River</td>
      <td>1948</td>
      <td>Passed</td>
      <td>133</td>
      <td>Action, Adventure, Drama</td>
      <td>7.8</td>
      <td>Dunson leads a cattle drive, the culmination o...</td>
      <td>77.97153</td>
      <td>Howard Hawks</td>
      <td>Arthur Rosson</td>
      <td>John Wayne</td>
      <td>Montgomery Clift</td>
      <td>Joanne Dru</td>
      <td>28167</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>710</th>
      <td>Key Largo</td>
      <td>1948</td>
      <td>Unknown</td>
      <td>100</td>
      <td>Action, Crime, Drama</td>
      <td>7.8</td>
      <td>A man visits his war buddy's family hotel and ...</td>
      <td>77.97153</td>
      <td>John Huston</td>
      <td>Humphrey Bogart</td>
      <td>Edward G. Robinson</td>
      <td>Lauren Bacall</td>
      <td>Lionel Barrymore</td>
      <td>36995</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>711</th>
      <td>To Have and Have Not</td>
      <td>1944</td>
      <td>PG</td>
      <td>100</td>
      <td>Adventure, Comedy, Film-Noir</td>
      <td>7.8</td>
      <td>During World War II, American expatriate Harry...</td>
      <td>77.97153</td>
      <td>Howard Hawks</td>
      <td>Humphrey Bogart</td>
      <td>Lauren Bacall</td>
      <td>Walter Brennan</td>
      <td>Dolores Moran</td>
      <td>31053</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>712</th>
      <td>Shadow of a Doubt</td>
      <td>1943</td>
      <td>PG</td>
      <td>108</td>
      <td>Film-Noir, Thriller</td>
      <td>7.8</td>
      <td>A young girl, overjoyed when her favorite uncl...</td>
      <td>94.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Teresa Wright</td>
      <td>Joseph Cotten</td>
      <td>Macdonald Carey</td>
      <td>Henry Travers</td>
      <td>59556</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>713</th>
      <td>Stagecoach</td>
      <td>1939</td>
      <td>Passed</td>
      <td>96</td>
      <td>Adventure, Drama, Western</td>
      <td>7.8</td>
      <td>A group of people traveling on a stagecoach fi...</td>
      <td>93.00000</td>
      <td>John Ford</td>
      <td>John Wayne</td>
      <td>Claire Trevor</td>
      <td>Andy Devine</td>
      <td>John Carradine</td>
      <td>43621</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>714</th>
      <td>The Lady Vanishes</td>
      <td>1938</td>
      <td>Unknown</td>
      <td>96</td>
      <td>Mystery, Thriller</td>
      <td>7.8</td>
      <td>While travelling in continental Europe, a rich...</td>
      <td>98.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Margaret Lockwood</td>
      <td>Michael Redgrave</td>
      <td>Paul Lukas</td>
      <td>May Whitty</td>
      <td>47400</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>715</th>
      <td>Bringing Up Baby</td>
      <td>1938</td>
      <td>Passed</td>
      <td>102</td>
      <td>Comedy, Family, Romance</td>
      <td>7.8</td>
      <td>While trying to secure a $1 million donation f...</td>
      <td>91.00000</td>
      <td>Howard Hawks</td>
      <td>Katharine Hepburn</td>
      <td>Cary Grant</td>
      <td>Charles Ruggles</td>
      <td>Walter Catlett</td>
      <td>55163</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>716</th>
      <td>Bride of Frankenstein</td>
      <td>1935</td>
      <td>Unknown</td>
      <td>75</td>
      <td>Drama, Horror, Sci-Fi</td>
      <td>7.8</td>
      <td>Mary Shelley reveals the main characters of he...</td>
      <td>95.00000</td>
      <td>James Whale</td>
      <td>Boris Karloff</td>
      <td>Elsa Lanchester</td>
      <td>Colin Clive</td>
      <td>Valerie Hobson</td>
      <td>43542</td>
      <td>4360000</td>
    </tr>
    <tr>
      <th>717</th>
      <td>Duck Soup</td>
      <td>1933</td>
      <td>Unknown</td>
      <td>69</td>
      <td>Comedy, Musical, War</td>
      <td>7.8</td>
      <td>Rufus T. Firefly is named president/dictator o...</td>
      <td>93.00000</td>
      <td>Leo McCarey</td>
      <td>Groucho Marx</td>
      <td>Harpo Marx</td>
      <td>Chico Marx</td>
      <td>Zeppo Marx</td>
      <td>55581</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>718</th>
      <td>Scarface: The Shame of the Nation</td>
      <td>1932</td>
      <td>PG</td>
      <td>93</td>
      <td>Action, Crime, Drama</td>
      <td>7.8</td>
      <td>An ambitious and nearly insane violent gangste...</td>
      <td>87.00000</td>
      <td>Howard Hawks</td>
      <td>Richard Rosson</td>
      <td>Paul Muni</td>
      <td>Ann Dvorak</td>
      <td>Karen Morley</td>
      <td>25312</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>719</th>
      <td>Frankenstein</td>
      <td>1931</td>
      <td>Passed</td>
      <td>70</td>
      <td>Drama, Horror, Sci-Fi</td>
      <td>7.8</td>
      <td>Dr. Frankenstein dares to tamper with life and...</td>
      <td>91.00000</td>
      <td>James Whale</td>
      <td>Colin Clive</td>
      <td>Mae Clarke</td>
      <td>Boris Karloff</td>
      <td>John Boles</td>
      <td>65341</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>720</th>
      <td>Roma</td>
      <td>2018</td>
      <td>R</td>
      <td>135</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>A year in the life of a middle-class family's ...</td>
      <td>96.00000</td>
      <td>Alfonso Cuarón</td>
      <td>Yalitza Aparicio</td>
      <td>Marina de Tavira</td>
      <td>Diego Cortina Autrey</td>
      <td>Carlos Peralta</td>
      <td>140375</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>721</th>
      <td>God's Own Country</td>
      <td>2017</td>
      <td>Unknown</td>
      <td>104</td>
      <td>Drama, Romance</td>
      <td>7.7</td>
      <td>Spring. Yorkshire. Young farmer Johnny Saxby n...</td>
      <td>85.00000</td>
      <td>Francis Lee</td>
      <td>Josh O'Connor</td>
      <td>Alec Secareanu</td>
      <td>Gemma Jones</td>
      <td>Ian Hart</td>
      <td>25198</td>
      <td>335609</td>
    </tr>
    <tr>
      <th>722</th>
      <td>Deadpool 2</td>
      <td>2018</td>
      <td>R</td>
      <td>119</td>
      <td>Action, Adventure, Comedy</td>
      <td>7.7</td>
      <td>Foul-mouthed mutant mercenary Wade Wilson (a.k...</td>
      <td>66.00000</td>
      <td>David Leitch</td>
      <td>Ryan Reynolds</td>
      <td>Josh Brolin</td>
      <td>Morena Baccarin</td>
      <td>Julian Dennison</td>
      <td>478586</td>
      <td>324591735</td>
    </tr>
    <tr>
      <th>723</th>
      <td>Wind River</td>
      <td>2017</td>
      <td>R</td>
      <td>107</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.7</td>
      <td>A veteran hunter helps an FBI agent investigat...</td>
      <td>73.00000</td>
      <td>Taylor Sheridan</td>
      <td>Kelsey Asbille</td>
      <td>Jeremy Renner</td>
      <td>Julia Jones</td>
      <td>Teo Briones</td>
      <td>205444</td>
      <td>33800859</td>
    </tr>
    <tr>
      <th>724</th>
      <td>Get Out</td>
      <td>2017</td>
      <td>R</td>
      <td>104</td>
      <td>Horror, Mystery, Thriller</td>
      <td>7.7</td>
      <td>A young African-American visits his white girl...</td>
      <td>85.00000</td>
      <td>Jordan Peele</td>
      <td>Daniel Kaluuya</td>
      <td>Allison Williams</td>
      <td>Bradley Whitford</td>
      <td>Catherine Keener</td>
      <td>492851</td>
      <td>176040665</td>
    </tr>
    <tr>
      <th>725</th>
      <td>Mission: Impossible - Fallout</td>
      <td>2018</td>
      <td>UA</td>
      <td>147</td>
      <td>Action, Adventure, Thriller</td>
      <td>7.7</td>
      <td>Ethan Hunt and his IMF team, along with some f...</td>
      <td>86.00000</td>
      <td>Christopher McQuarrie</td>
      <td>Tom Cruise</td>
      <td>Henry Cavill</td>
      <td>Ving Rhames</td>
      <td>Simon Pegg</td>
      <td>291257</td>
      <td>220159104</td>
    </tr>
    <tr>
      <th>726</th>
      <td>En man som heter Ove</td>
      <td>2015</td>
      <td>PG-13</td>
      <td>116</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>Ove, an ill-tempered, isolated retiree who spe...</td>
      <td>70.00000</td>
      <td>Hannes Holm</td>
      <td>Rolf Lassgård</td>
      <td>Bahar Pars</td>
      <td>Filip Berg</td>
      <td>Ida Engvoll</td>
      <td>47444</td>
      <td>3358518</td>
    </tr>
    <tr>
      <th>727</th>
      <td>What We Do in the Shadows</td>
      <td>2014</td>
      <td>R</td>
      <td>86</td>
      <td>Comedy, Horror</td>
      <td>7.7</td>
      <td>Viago, Deacon and Vladislav are vampires who a...</td>
      <td>76.00000</td>
      <td>Jemaine Clement</td>
      <td>Taika Waititi</td>
      <td>Jemaine Clement</td>
      <td>Taika Waititi</td>
      <td>Cori Gonzalez-Macuer</td>
      <td>157498</td>
      <td>3333000</td>
    </tr>
    <tr>
      <th>728</th>
      <td>Omoide no Mânî</td>
      <td>2014</td>
      <td>U</td>
      <td>103</td>
      <td>Animation, Drama, Family</td>
      <td>7.7</td>
      <td>Due to 12 y.o. Anna's asthma, she's sent to st...</td>
      <td>72.00000</td>
      <td>James Simone</td>
      <td>Hiromasa Yonebayashi</td>
      <td>Sara Takatsuki</td>
      <td>Kasumi Arimura</td>
      <td>Nanako Matsushima</td>
      <td>32798</td>
      <td>765127</td>
    </tr>
    <tr>
      <th>729</th>
      <td>The Theory of Everything</td>
      <td>2014</td>
      <td>U</td>
      <td>123</td>
      <td>Biography, Drama, Romance</td>
      <td>7.7</td>
      <td>A look at the relationship between the famous ...</td>
      <td>72.00000</td>
      <td>James Marsh</td>
      <td>Eddie Redmayne</td>
      <td>Felicity Jones</td>
      <td>Tom Prior</td>
      <td>Sophie Perry</td>
      <td>404182</td>
      <td>35893537</td>
    </tr>
    <tr>
      <th>730</th>
      <td>Kingsman: The Secret Service</td>
      <td>2014</td>
      <td>A</td>
      <td>129</td>
      <td>Action, Adventure, Comedy</td>
      <td>7.7</td>
      <td>A spy organisation recruits a promising street...</td>
      <td>60.00000</td>
      <td>Matthew Vaughn</td>
      <td>Colin Firth</td>
      <td>Taron Egerton</td>
      <td>Samuel L. Jackson</td>
      <td>Michael Caine</td>
      <td>590440</td>
      <td>128261724</td>
    </tr>
    <tr>
      <th>731</th>
      <td>The Fault in Our Stars</td>
      <td>2014</td>
      <td>UA</td>
      <td>126</td>
      <td>Drama, Romance</td>
      <td>7.7</td>
      <td>Two teenage cancer patients begin a life-affir...</td>
      <td>69.00000</td>
      <td>Josh Boone</td>
      <td>Shailene Woodley</td>
      <td>Ansel Elgort</td>
      <td>Nat Wolff</td>
      <td>Laura Dern</td>
      <td>344312</td>
      <td>124872350</td>
    </tr>
    <tr>
      <th>732</th>
      <td>Me and Earl and the Dying Girl</td>
      <td>2015</td>
      <td>PG-13</td>
      <td>105</td>
      <td>Comedy, Drama</td>
      <td>7.7</td>
      <td>High schooler Greg, who spends most of his tim...</td>
      <td>74.00000</td>
      <td>Alfonso Gomez-Rejon</td>
      <td>Thomas Mann</td>
      <td>RJ Cyler</td>
      <td>Olivia Cooke</td>
      <td>Nick Offerman</td>
      <td>123210</td>
      <td>6743776</td>
    </tr>
    <tr>
      <th>733</th>
      <td>Birdman or (The Unexpected Virtue of Ignorance)</td>
      <td>2014</td>
      <td>A</td>
      <td>119</td>
      <td>Comedy, Drama</td>
      <td>7.7</td>
      <td>A washed-up superhero actor attempts to revive...</td>
      <td>87.00000</td>
      <td>Alejandro G. Iñárritu</td>
      <td>Michael Keaton</td>
      <td>Zach Galifianakis</td>
      <td>Edward Norton</td>
      <td>Andrea Riseborough</td>
      <td>580291</td>
      <td>42340598</td>
    </tr>
    <tr>
      <th>734</th>
      <td>La vie d'Adèle</td>
      <td>2013</td>
      <td>A</td>
      <td>180</td>
      <td>Drama, Romance</td>
      <td>7.7</td>
      <td>Adèle's life is changed when she meets Emma, a...</td>
      <td>89.00000</td>
      <td>Abdellatif Kechiche</td>
      <td>Léa Seydoux</td>
      <td>Adèle Exarchopoulos</td>
      <td>Salim Kechiouche</td>
      <td>Aurélien Recoing</td>
      <td>138741</td>
      <td>2199675</td>
    </tr>
    <tr>
      <th>735</th>
      <td>Kai po che!</td>
      <td>2013</td>
      <td>U</td>
      <td>130</td>
      <td>Drama, Sport</td>
      <td>7.7</td>
      <td>Three friends growing up in India at the turn ...</td>
      <td>40.00000</td>
      <td>Abhishek Kapoor</td>
      <td>Amit Sadh</td>
      <td>Sushant Singh Rajput</td>
      <td>Rajkummar Rao</td>
      <td>Amrita Puri</td>
      <td>32628</td>
      <td>1122527</td>
    </tr>
    <tr>
      <th>736</th>
      <td>The Broken Circle Breakdown</td>
      <td>2012</td>
      <td>Unknown</td>
      <td>111</td>
      <td>Drama, Music, Romance</td>
      <td>7.7</td>
      <td>Elise and Didier fall in love at first sight, ...</td>
      <td>70.00000</td>
      <td>Felix van Groeningen</td>
      <td>Veerle Baetens</td>
      <td>Johan Heldenbergh</td>
      <td>Nell Cattrysse</td>
      <td>Geert Van Rampelberg</td>
      <td>39379</td>
      <td>175058</td>
    </tr>
    <tr>
      <th>737</th>
      <td>Captain America: The Winter Soldier</td>
      <td>2014</td>
      <td>UA</td>
      <td>136</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.7</td>
      <td>As Steve Rogers struggles to embrace his role ...</td>
      <td>70.00000</td>
      <td>Anthony Russo</td>
      <td>Joe Russo</td>
      <td>Chris Evans</td>
      <td>Samuel L. Jackson</td>
      <td>Scarlett Johansson</td>
      <td>736182</td>
      <td>259766572</td>
    </tr>
    <tr>
      <th>738</th>
      <td>Rockstar</td>
      <td>2011</td>
      <td>UA</td>
      <td>159</td>
      <td>Drama, Music, Musical</td>
      <td>7.7</td>
      <td>Janardhan Jakhar chases his dreams of becoming...</td>
      <td>77.97153</td>
      <td>Imtiaz Ali</td>
      <td>Ranbir Kapoor</td>
      <td>Nargis Fakhri</td>
      <td>Shammi Kapoor</td>
      <td>Kumud Mishra</td>
      <td>39501</td>
      <td>985912</td>
    </tr>
    <tr>
      <th>739</th>
      <td>Nebraska</td>
      <td>2013</td>
      <td>UA</td>
      <td>115</td>
      <td>Adventure, Comedy, Drama</td>
      <td>7.7</td>
      <td>An aging, booze-addled father makes the trip f...</td>
      <td>87.00000</td>
      <td>Alexander Payne</td>
      <td>Bruce Dern</td>
      <td>Will Forte</td>
      <td>June Squibb</td>
      <td>Bob Odenkirk</td>
      <td>112298</td>
      <td>17654912</td>
    </tr>
    <tr>
      <th>740</th>
      <td>Wreck-It Ralph</td>
      <td>2012</td>
      <td>U</td>
      <td>101</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.7</td>
      <td>A video game villain wants to be a hero and se...</td>
      <td>72.00000</td>
      <td>Rich Moore</td>
      <td>John C. Reilly</td>
      <td>Jack McBrayer</td>
      <td>Jane Lynch</td>
      <td>Sarah Silverman</td>
      <td>380195</td>
      <td>189422889</td>
    </tr>
    <tr>
      <th>741</th>
      <td>Le Petit Prince</td>
      <td>2015</td>
      <td>PG</td>
      <td>108</td>
      <td>Animation, Adventure, Drama</td>
      <td>7.7</td>
      <td>A little girl lives in a very grown-up world w...</td>
      <td>70.00000</td>
      <td>Mark Osborne</td>
      <td>Jeff Bridges</td>
      <td>Mackenzie Foy</td>
      <td>Rachel McAdams</td>
      <td>Marion Cotillard</td>
      <td>56720</td>
      <td>1339152</td>
    </tr>
    <tr>
      <th>742</th>
      <td>Detachment</td>
      <td>2011</td>
      <td>Unknown</td>
      <td>98</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>A substitute teacher who drifts from classroom...</td>
      <td>52.00000</td>
      <td>Tony Kaye</td>
      <td>Adrien Brody</td>
      <td>Christina Hendricks</td>
      <td>Marcia Gay Harden</td>
      <td>Lucy Liu</td>
      <td>77071</td>
      <td>71177</td>
    </tr>
    <tr>
      <th>743</th>
      <td>Midnight in Paris</td>
      <td>2011</td>
      <td>PG-13</td>
      <td>96</td>
      <td>Comedy, Fantasy, Romance</td>
      <td>7.7</td>
      <td>While on a trip to Paris with his fiancée's fa...</td>
      <td>81.00000</td>
      <td>Woody Allen</td>
      <td>Owen Wilson</td>
      <td>Rachel McAdams</td>
      <td>Kathy Bates</td>
      <td>Kurt Fuller</td>
      <td>388089</td>
      <td>56816662</td>
    </tr>
    <tr>
      <th>744</th>
      <td>The Lego Movie</td>
      <td>2014</td>
      <td>U</td>
      <td>100</td>
      <td>Animation, Action, Adventure</td>
      <td>7.7</td>
      <td>An ordinary LEGO construction worker, thought ...</td>
      <td>83.00000</td>
      <td>Christopher Miller</td>
      <td>Phil Lord</td>
      <td>Chris Pratt</td>
      <td>Will Ferrell</td>
      <td>Elizabeth Banks</td>
      <td>323982</td>
      <td>257760692</td>
    </tr>
    <tr>
      <th>745</th>
      <td>Gravity</td>
      <td>2013</td>
      <td>UA</td>
      <td>91</td>
      <td>Drama, Sci-Fi, Thriller</td>
      <td>7.7</td>
      <td>Two astronauts work together to survive after ...</td>
      <td>96.00000</td>
      <td>Alfonso Cuarón</td>
      <td>Sandra Bullock</td>
      <td>George Clooney</td>
      <td>Ed Harris</td>
      <td>Orto Ignatiussen</td>
      <td>769145</td>
      <td>274092705</td>
    </tr>
    <tr>
      <th>746</th>
      <td>Star Trek Into Darkness</td>
      <td>2013</td>
      <td>UA</td>
      <td>132</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.7</td>
      <td>After the crew of the Enterprise find an unsto...</td>
      <td>72.00000</td>
      <td>J.J. Abrams</td>
      <td>Chris Pine</td>
      <td>Zachary Quinto</td>
      <td>Zoe Saldana</td>
      <td>Benedict Cumberbatch</td>
      <td>463188</td>
      <td>228778661</td>
    </tr>
    <tr>
      <th>747</th>
      <td>Beasts of No Nation</td>
      <td>2015</td>
      <td>Unknown</td>
      <td>137</td>
      <td>Drama, War</td>
      <td>7.7</td>
      <td>A drama based on the experiences of Agu, a chi...</td>
      <td>79.00000</td>
      <td>Cary Joji Fukunaga</td>
      <td>Abraham Attah</td>
      <td>Emmanuel Affadzi</td>
      <td>Ricky Adelayitor</td>
      <td>Andrew Adote</td>
      <td>73964</td>
      <td>83861</td>
    </tr>
    <tr>
      <th>748</th>
      <td>The Social Network</td>
      <td>2010</td>
      <td>UA</td>
      <td>120</td>
      <td>Biography, Drama</td>
      <td>7.7</td>
      <td>As Harvard student Mark Zuckerberg creates the...</td>
      <td>95.00000</td>
      <td>David Fincher</td>
      <td>Jesse Eisenberg</td>
      <td>Andrew Garfield</td>
      <td>Justin Timberlake</td>
      <td>Rooney Mara</td>
      <td>624982</td>
      <td>96962694</td>
    </tr>
    <tr>
      <th>749</th>
      <td>X: First Class</td>
      <td>2011</td>
      <td>UA</td>
      <td>131</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.7</td>
      <td>In the 1960s, superpowered humans Charles Xavi...</td>
      <td>65.00000</td>
      <td>Matthew Vaughn</td>
      <td>James McAvoy</td>
      <td>Michael Fassbender</td>
      <td>Jennifer Lawrence</td>
      <td>Kevin Bacon</td>
      <td>645512</td>
      <td>146408305</td>
    </tr>
    <tr>
      <th>750</th>
      <td>The Hangover</td>
      <td>2009</td>
      <td>UA</td>
      <td>100</td>
      <td>Comedy</td>
      <td>7.7</td>
      <td>Three buddies wake up from a bachelor party in...</td>
      <td>73.00000</td>
      <td>Todd Phillips</td>
      <td>Zach Galifianakis</td>
      <td>Bradley Cooper</td>
      <td>Justin Bartha</td>
      <td>Ed Helms</td>
      <td>717559</td>
      <td>277322503</td>
    </tr>
    <tr>
      <th>751</th>
      <td>Skyfall</td>
      <td>2012</td>
      <td>UA</td>
      <td>143</td>
      <td>Action, Adventure, Thriller</td>
      <td>7.7</td>
      <td>James Bond's loyalty to M is tested when her p...</td>
      <td>81.00000</td>
      <td>Sam Mendes</td>
      <td>Daniel Craig</td>
      <td>Javier Bardem</td>
      <td>Naomie Harris</td>
      <td>Judi Dench</td>
      <td>630614</td>
      <td>304360277</td>
    </tr>
    <tr>
      <th>752</th>
      <td>Silver Linings Playbook</td>
      <td>2012</td>
      <td>A</td>
      <td>122</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>After a stint in a mental institution, former ...</td>
      <td>81.00000</td>
      <td>David O. Russell</td>
      <td>Bradley Cooper</td>
      <td>Jennifer Lawrence</td>
      <td>Robert De Niro</td>
      <td>Jacki Weaver</td>
      <td>661871</td>
      <td>132092958</td>
    </tr>
    <tr>
      <th>753</th>
      <td>Argo</td>
      <td>2012</td>
      <td>A</td>
      <td>120</td>
      <td>Biography, Drama, Thriller</td>
      <td>7.7</td>
      <td>Acting under the cover of a Hollywood producer...</td>
      <td>86.00000</td>
      <td>Ben Affleck</td>
      <td>Ben Affleck</td>
      <td>Bryan Cranston</td>
      <td>John Goodman</td>
      <td>Alan Arkin</td>
      <td>572581</td>
      <td>136025503</td>
    </tr>
    <tr>
      <th>754</th>
      <td>(500) Days of Summer</td>
      <td>2009</td>
      <td>UA</td>
      <td>95</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>An offbeat romantic comedy about a woman who d...</td>
      <td>76.00000</td>
      <td>Marc Webb</td>
      <td>Zooey Deschanel</td>
      <td>Joseph Gordon-Levitt</td>
      <td>Geoffrey Arend</td>
      <td>Chloë Grace Moretz</td>
      <td>472242</td>
      <td>32391374</td>
    </tr>
    <tr>
      <th>755</th>
      <td>Harry Potter and the Deathly Hallows: Part 1</td>
      <td>2010</td>
      <td>A</td>
      <td>146</td>
      <td>Adventure, Family, Fantasy</td>
      <td>7.7</td>
      <td>As Harry, Ron, and Hermione race against time ...</td>
      <td>65.00000</td>
      <td>David Yates</td>
      <td>Daniel Radcliffe</td>
      <td>Emma Watson</td>
      <td>Rupert Grint</td>
      <td>Bill Nighy</td>
      <td>479120</td>
      <td>295983305</td>
    </tr>
    <tr>
      <th>756</th>
      <td>Gake no ue no Ponyo</td>
      <td>2008</td>
      <td>U</td>
      <td>101</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.7</td>
      <td>A five-year-old boy develops a relationship wi...</td>
      <td>86.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Cate Blanchett</td>
      <td>Matt Damon</td>
      <td>Liam Neeson</td>
      <td>Tomoko Yamaguchi</td>
      <td>125317</td>
      <td>15090400</td>
    </tr>
    <tr>
      <th>757</th>
      <td>Frost/Nixon</td>
      <td>2008</td>
      <td>R</td>
      <td>122</td>
      <td>Biography, Drama, History</td>
      <td>7.7</td>
      <td>A dramatic retelling of the post-Watergate tel...</td>
      <td>80.00000</td>
      <td>Ron Howard</td>
      <td>Frank Langella</td>
      <td>Michael Sheen</td>
      <td>Kevin Bacon</td>
      <td>Sam Rockwell</td>
      <td>103330</td>
      <td>18593156</td>
    </tr>
    <tr>
      <th>758</th>
      <td>Papurika</td>
      <td>2006</td>
      <td>U</td>
      <td>90</td>
      <td>Animation, Drama, Fantasy</td>
      <td>7.7</td>
      <td>When a machine that allows therapists to enter...</td>
      <td>81.00000</td>
      <td>Satoshi Kon</td>
      <td>Megumi Hayashibara</td>
      <td>Tôru Emori</td>
      <td>Katsunosuke Hori</td>
      <td>Tôru Furuya</td>
      <td>71379</td>
      <td>881302</td>
    </tr>
    <tr>
      <th>759</th>
      <td>Changeling</td>
      <td>2008</td>
      <td>R</td>
      <td>141</td>
      <td>Biography, Crime, Drama</td>
      <td>7.7</td>
      <td>Grief-stricken mother Christine Collins (Angel...</td>
      <td>63.00000</td>
      <td>Clint Eastwood</td>
      <td>Angelina Jolie</td>
      <td>Colm Feore</td>
      <td>Amy Ryan</td>
      <td>Gattlin Griffith</td>
      <td>239203</td>
      <td>35739802</td>
    </tr>
    <tr>
      <th>760</th>
      <td>Flipped</td>
      <td>2010</td>
      <td>PG</td>
      <td>90</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>Two eighth-graders start to have feelings for ...</td>
      <td>45.00000</td>
      <td>Rob Reiner</td>
      <td>Madeline Carroll</td>
      <td>Callan McAuliffe</td>
      <td>Rebecca De Mornay</td>
      <td>Anthony Edwards</td>
      <td>81446</td>
      <td>1752214</td>
    </tr>
    <tr>
      <th>761</th>
      <td>Toki o kakeru shôjo</td>
      <td>2006</td>
      <td>U</td>
      <td>98</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.7</td>
      <td>A high-school girl named Makoto acquires the p...</td>
      <td>77.97153</td>
      <td>Mamoru Hosoda</td>
      <td>Riisa Naka</td>
      <td>Takuya Ishida</td>
      <td>Mitsutaka Itakura</td>
      <td>Ayami Kakiuchi</td>
      <td>60368</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>762</th>
      <td>Death Note: Desu nôto</td>
      <td>2006</td>
      <td>Unknown</td>
      <td>126</td>
      <td>Crime, Drama, Fantasy</td>
      <td>7.7</td>
      <td>A battle between the world's two greatest mind...</td>
      <td>77.97153</td>
      <td>Shûsuke Kaneko</td>
      <td>Tatsuya Fujiwara</td>
      <td>Ken'ichi Matsuyama</td>
      <td>Asaka Seto</td>
      <td>Yû Kashii</td>
      <td>28630</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>763</th>
      <td>This Is England</td>
      <td>2006</td>
      <td>Unknown</td>
      <td>101</td>
      <td>Crime, Drama</td>
      <td>7.7</td>
      <td>A young boy becomes friends with a gang of ski...</td>
      <td>86.00000</td>
      <td>Shane Meadows</td>
      <td>Thomas Turgoose</td>
      <td>Stephen Graham</td>
      <td>Jo Hartley</td>
      <td>Andrew Shim</td>
      <td>115576</td>
      <td>327919</td>
    </tr>
    <tr>
      <th>764</th>
      <td>Ex Machina</td>
      <td>2014</td>
      <td>UA</td>
      <td>108</td>
      <td>Drama, Sci-Fi, Thriller</td>
      <td>7.7</td>
      <td>A young programmer is selected to participate ...</td>
      <td>78.00000</td>
      <td>Alex Garland</td>
      <td>Alicia Vikander</td>
      <td>Domhnall Gleeson</td>
      <td>Oscar Isaac</td>
      <td>Sonoya Mizuno</td>
      <td>474141</td>
      <td>25442958</td>
    </tr>
    <tr>
      <th>765</th>
      <td>Efter brylluppet</td>
      <td>2006</td>
      <td>R</td>
      <td>120</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>A manager of an orphanage in India is sent to ...</td>
      <td>78.00000</td>
      <td>Susanne Bier</td>
      <td>Mads Mikkelsen</td>
      <td>Sidse Babett Knudsen</td>
      <td>Rolf Lassgård</td>
      <td>Neeral Mulchandani</td>
      <td>32001</td>
      <td>412544</td>
    </tr>
    <tr>
      <th>766</th>
      <td>The Last King of Scotland</td>
      <td>2006</td>
      <td>R</td>
      <td>123</td>
      <td>Biography, Drama, History</td>
      <td>7.7</td>
      <td>Based on the events of the brutal Ugandan dict...</td>
      <td>74.00000</td>
      <td>Kevin Macdonald</td>
      <td>James McAvoy</td>
      <td>Forest Whitaker</td>
      <td>Gillian Anderson</td>
      <td>Kerry Washington</td>
      <td>175355</td>
      <td>17605861</td>
    </tr>
    <tr>
      <th>767</th>
      <td>Zodiac</td>
      <td>2007</td>
      <td>UA</td>
      <td>157</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.7</td>
      <td>In the late 1960s/early 1970s, a San Francisco...</td>
      <td>78.00000</td>
      <td>David Fincher</td>
      <td>Jake Gyllenhaal</td>
      <td>Robert Downey Jr.</td>
      <td>Mark Ruffalo</td>
      <td>Anthony Edwards</td>
      <td>466080</td>
      <td>33080084</td>
    </tr>
    <tr>
      <th>768</th>
      <td>Lucky Number Slevin</td>
      <td>2006</td>
      <td>R</td>
      <td>110</td>
      <td>Action, Crime, Drama</td>
      <td>7.7</td>
      <td>A case of mistaken identity lands Slevin into ...</td>
      <td>53.00000</td>
      <td>Paul McGuigan</td>
      <td>Josh Hartnett</td>
      <td>Ben Kingsley</td>
      <td>Morgan Freeman</td>
      <td>Lucy Liu</td>
      <td>299524</td>
      <td>22494487</td>
    </tr>
    <tr>
      <th>769</th>
      <td>Joyeux Noël</td>
      <td>2005</td>
      <td>PG-13</td>
      <td>116</td>
      <td>Drama, History, Music</td>
      <td>7.7</td>
      <td>In December 1914, an unofficial Christmas truc...</td>
      <td>70.00000</td>
      <td>Christian Carion</td>
      <td>Diane Kruger</td>
      <td>Benno Fürmann</td>
      <td>Guillaume Canet</td>
      <td>Natalie Dessay</td>
      <td>28003</td>
      <td>1054361</td>
    </tr>
    <tr>
      <th>770</th>
      <td>Control</td>
      <td>2007</td>
      <td>R</td>
      <td>122</td>
      <td>Biography, Drama, Music</td>
      <td>7.7</td>
      <td>A profile of Ian Curtis, the enigmatic singer ...</td>
      <td>78.00000</td>
      <td>Anton Corbijn</td>
      <td>Sam Riley</td>
      <td>Samantha Morton</td>
      <td>Craig Parkinson</td>
      <td>Alexandra Maria Lara</td>
      <td>61609</td>
      <td>871577</td>
    </tr>
    <tr>
      <th>771</th>
      <td>Tangled</td>
      <td>2010</td>
      <td>U</td>
      <td>100</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.7</td>
      <td>The magically long-haired Rapunzel has spent h...</td>
      <td>71.00000</td>
      <td>Nathan Greno</td>
      <td>Byron Howard</td>
      <td>Mandy Moore</td>
      <td>Zachary Levi</td>
      <td>Donna Murphy</td>
      <td>405922</td>
      <td>200821936</td>
    </tr>
    <tr>
      <th>772</th>
      <td>Zwartboek</td>
      <td>2006</td>
      <td>R</td>
      <td>145</td>
      <td>Drama, Thriller, War</td>
      <td>7.7</td>
      <td>In the Nazi-occupied Netherlands during World ...</td>
      <td>71.00000</td>
      <td>Paul Verhoeven</td>
      <td>Carice van Houten</td>
      <td>Sebastian Koch</td>
      <td>Thom Hoffman</td>
      <td>Halina Reijn</td>
      <td>72643</td>
      <td>4398392</td>
    </tr>
    <tr>
      <th>773</th>
      <td>Brokeback Mountain</td>
      <td>2005</td>
      <td>A</td>
      <td>134</td>
      <td>Drama, Romance</td>
      <td>7.7</td>
      <td>The story of a forbidden and secretive relatio...</td>
      <td>87.00000</td>
      <td>Ang Lee</td>
      <td>Jake Gyllenhaal</td>
      <td>Heath Ledger</td>
      <td>Michelle Williams</td>
      <td>Randy Quaid</td>
      <td>323103</td>
      <td>83043761</td>
    </tr>
    <tr>
      <th>774</th>
      <td>3:10 to Yuma</td>
      <td>2007</td>
      <td>A</td>
      <td>122</td>
      <td>Action, Crime, Drama</td>
      <td>7.7</td>
      <td>A small-time rancher agrees to hold a captured...</td>
      <td>76.00000</td>
      <td>James Mangold</td>
      <td>Russell Crowe</td>
      <td>Christian Bale</td>
      <td>Ben Foster</td>
      <td>Logan Lerman</td>
      <td>288797</td>
      <td>53606916</td>
    </tr>
    <tr>
      <th>775</th>
      <td>Crash</td>
      <td>2004</td>
      <td>UA</td>
      <td>112</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.7</td>
      <td>Los Angeles citizens with vastly separate live...</td>
      <td>66.00000</td>
      <td>Paul Haggis</td>
      <td>Don Cheadle</td>
      <td>Sandra Bullock</td>
      <td>Thandie Newton</td>
      <td>Karina Arroyave</td>
      <td>419483</td>
      <td>54580300</td>
    </tr>
    <tr>
      <th>776</th>
      <td>Kung fu</td>
      <td>2004</td>
      <td>UA</td>
      <td>99</td>
      <td>Action, Comedy, Fantasy</td>
      <td>7.7</td>
      <td>In Shanghai, China in the 1940s, a wannabe gan...</td>
      <td>78.00000</td>
      <td>Stephen Chow</td>
      <td>Stephen Chow</td>
      <td>Wah Yuen</td>
      <td>Qiu Yuen</td>
      <td>Siu-Lung Leung</td>
      <td>127250</td>
      <td>17108591</td>
    </tr>
    <tr>
      <th>777</th>
      <td>The Bourne Supremacy</td>
      <td>2004</td>
      <td>A</td>
      <td>108</td>
      <td>Action, Mystery, Thriller</td>
      <td>7.7</td>
      <td>When Jason Bourne is framed for a CIA operatio...</td>
      <td>73.00000</td>
      <td>Paul Greengrass</td>
      <td>Matt Damon</td>
      <td>Franka Potente</td>
      <td>Joan Allen</td>
      <td>Brian Cox</td>
      <td>434841</td>
      <td>176241941</td>
    </tr>
    <tr>
      <th>778</th>
      <td>The Machinist</td>
      <td>2004</td>
      <td>R</td>
      <td>101</td>
      <td>Drama, Thriller</td>
      <td>7.7</td>
      <td>An industrial worker who hasn't slept in a yea...</td>
      <td>61.00000</td>
      <td>Brad Anderson</td>
      <td>Christian Bale</td>
      <td>Jennifer Jason Leigh</td>
      <td>Aitana Sánchez-Gijón</td>
      <td>John Sharian</td>
      <td>358432</td>
      <td>1082715</td>
    </tr>
    <tr>
      <th>779</th>
      <td>Ray</td>
      <td>2004</td>
      <td>A</td>
      <td>152</td>
      <td>Biography, Drama, Music</td>
      <td>7.7</td>
      <td>The story of the life and career of the legend...</td>
      <td>73.00000</td>
      <td>Taylor Hackford</td>
      <td>Jamie Foxx</td>
      <td>Regina King</td>
      <td>Kerry Washington</td>
      <td>Clifton Powell</td>
      <td>138356</td>
      <td>75331600</td>
    </tr>
    <tr>
      <th>780</th>
      <td>Lost in Translation</td>
      <td>2003</td>
      <td>UA</td>
      <td>102</td>
      <td>Comedy, Drama</td>
      <td>7.7</td>
      <td>A faded movie star and a neglected young woman...</td>
      <td>89.00000</td>
      <td>Sofia Coppola</td>
      <td>Bill Murray</td>
      <td>Scarlett Johansson</td>
      <td>Giovanni Ribisi</td>
      <td>Anna Faris</td>
      <td>415074</td>
      <td>44585453</td>
    </tr>
    <tr>
      <th>781</th>
      <td>Harry Potter and the Goblet of Fire</td>
      <td>2005</td>
      <td>UA</td>
      <td>157</td>
      <td>Adventure, Family, Fantasy</td>
      <td>7.7</td>
      <td>Harry Potter finds himself competing in a haza...</td>
      <td>81.00000</td>
      <td>Mike Newell</td>
      <td>Daniel Radcliffe</td>
      <td>Emma Watson</td>
      <td>Rupert Grint</td>
      <td>Eric Sykes</td>
      <td>548619</td>
      <td>290013036</td>
    </tr>
    <tr>
      <th>782</th>
      <td>Man on Fire</td>
      <td>2004</td>
      <td>UA</td>
      <td>146</td>
      <td>Action, Crime, Drama</td>
      <td>7.7</td>
      <td>In Mexico City, a former CIA operative swears ...</td>
      <td>47.00000</td>
      <td>Tony Scott</td>
      <td>Denzel Washington</td>
      <td>Christopher Walken</td>
      <td>Dakota Fanning</td>
      <td>Radha Mitchell</td>
      <td>329592</td>
      <td>77911774</td>
    </tr>
    <tr>
      <th>783</th>
      <td>Coraline</td>
      <td>2009</td>
      <td>U</td>
      <td>100</td>
      <td>Animation, Drama, Family</td>
      <td>7.7</td>
      <td>An adventurous 11-year-old girl finds another ...</td>
      <td>80.00000</td>
      <td>Henry Selick</td>
      <td>Dakota Fanning</td>
      <td>Teri Hatcher</td>
      <td>John Hodgman</td>
      <td>Jennifer Saunders</td>
      <td>197761</td>
      <td>75286229</td>
    </tr>
    <tr>
      <th>784</th>
      <td>The Last Samurai</td>
      <td>2003</td>
      <td>UA</td>
      <td>154</td>
      <td>Action, Drama</td>
      <td>7.7</td>
      <td>An American military advisor embraces the Samu...</td>
      <td>55.00000</td>
      <td>Edward Zwick</td>
      <td>Tom Cruise</td>
      <td>Ken Watanabe</td>
      <td>Billy Connolly</td>
      <td>William Atherton</td>
      <td>400049</td>
      <td>111110575</td>
    </tr>
    <tr>
      <th>785</th>
      <td>The Magdalene Sisters</td>
      <td>2002</td>
      <td>R</td>
      <td>114</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>Three young Irish women struggle to maintain t...</td>
      <td>83.00000</td>
      <td>Peter Mullan</td>
      <td>Eileen Walsh</td>
      <td>Dorothy Duffy</td>
      <td>Nora-Jane Noone</td>
      <td>Anne-Marie Duff</td>
      <td>25938</td>
      <td>4890878</td>
    </tr>
    <tr>
      <th>786</th>
      <td>Good Bye Lenin!</td>
      <td>2003</td>
      <td>R</td>
      <td>121</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>In 1990, to protect his fragile mother from a ...</td>
      <td>68.00000</td>
      <td>Wolfgang Becker</td>
      <td>Daniel Brühl</td>
      <td>Katrin Saß</td>
      <td>Chulpan Khamatova</td>
      <td>Florian Lukas</td>
      <td>137981</td>
      <td>4064200</td>
    </tr>
    <tr>
      <th>787</th>
      <td>In America</td>
      <td>2002</td>
      <td>PG-13</td>
      <td>105</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>A family of Irish immigrants adjust to life on...</td>
      <td>76.00000</td>
      <td>Jim Sheridan</td>
      <td>Paddy Considine</td>
      <td>Samantha Morton</td>
      <td>Djimon Hounsou</td>
      <td>Sarah Bolger</td>
      <td>40403</td>
      <td>15539266</td>
    </tr>
    <tr>
      <th>788</th>
      <td>I Am Sam</td>
      <td>2001</td>
      <td>PG-13</td>
      <td>132</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>A mentally handicapped man fights for custody ...</td>
      <td>28.00000</td>
      <td>Jessie Nelson</td>
      <td>Sean Penn</td>
      <td>Michelle Pfeiffer</td>
      <td>Dakota Fanning</td>
      <td>Dianne Wiest</td>
      <td>142863</td>
      <td>40311852</td>
    </tr>
    <tr>
      <th>789</th>
      <td>Adaptation.</td>
      <td>2002</td>
      <td>R</td>
      <td>115</td>
      <td>Comedy, Drama</td>
      <td>7.7</td>
      <td>A lovelorn screenwriter becomes desperate as h...</td>
      <td>83.00000</td>
      <td>Spike Jonze</td>
      <td>Nicolas Cage</td>
      <td>Meryl Streep</td>
      <td>Chris Cooper</td>
      <td>Tilda Swinton</td>
      <td>178565</td>
      <td>22245861</td>
    </tr>
    <tr>
      <th>790</th>
      <td>Black Hawk Down</td>
      <td>2001</td>
      <td>A</td>
      <td>144</td>
      <td>Drama, History, War</td>
      <td>7.7</td>
      <td>160 elite U.S. soldiers drop into Somalia to c...</td>
      <td>74.00000</td>
      <td>Ridley Scott</td>
      <td>Josh Hartnett</td>
      <td>Ewan McGregor</td>
      <td>Tom Sizemore</td>
      <td>Eric Bana</td>
      <td>364254</td>
      <td>108638745</td>
    </tr>
    <tr>
      <th>791</th>
      <td>Road to Perdition</td>
      <td>2002</td>
      <td>A</td>
      <td>117</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.7</td>
      <td>A mob enforcer's son witnesses a murder, forci...</td>
      <td>72.00000</td>
      <td>Sam Mendes</td>
      <td>Tom Hanks</td>
      <td>Tyler Hoechlin</td>
      <td>Rob Maxey</td>
      <td>Liam Aiken</td>
      <td>246840</td>
      <td>104454762</td>
    </tr>
    <tr>
      <th>792</th>
      <td>Das Experiment</td>
      <td>2001</td>
      <td>R</td>
      <td>120</td>
      <td>Drama, Thriller</td>
      <td>7.7</td>
      <td>For two weeks, 20 male participants are hired ...</td>
      <td>60.00000</td>
      <td>Oliver Hirschbiegel</td>
      <td>Moritz Bleibtreu</td>
      <td>Christian Berkel</td>
      <td>Oliver Stokowski</td>
      <td>Wotan Wilke Möhring</td>
      <td>90842</td>
      <td>141072</td>
    </tr>
    <tr>
      <th>793</th>
      <td>Billy Elliot</td>
      <td>2000</td>
      <td>R</td>
      <td>110</td>
      <td>Drama, Music</td>
      <td>7.7</td>
      <td>A talented young boy becomes torn between his ...</td>
      <td>74.00000</td>
      <td>Stephen Daldry</td>
      <td>Jamie Bell</td>
      <td>Julie Walters</td>
      <td>Jean Heywood</td>
      <td>Jamie Draven</td>
      <td>126770</td>
      <td>21995263</td>
    </tr>
    <tr>
      <th>794</th>
      <td>Hedwig and the Angry Inch</td>
      <td>2001</td>
      <td>R</td>
      <td>95</td>
      <td>Comedy, Drama, Music</td>
      <td>7.7</td>
      <td>A gender-queer punk-rock singer from East Berl...</td>
      <td>85.00000</td>
      <td>John Cameron Mitchell</td>
      <td>John Cameron Mitchell</td>
      <td>Miriam Shor</td>
      <td>Stephen Trask</td>
      <td>Theodore Liscinski</td>
      <td>31957</td>
      <td>3029081</td>
    </tr>
    <tr>
      <th>795</th>
      <td>Ocean's Eleven</td>
      <td>2001</td>
      <td>UA</td>
      <td>116</td>
      <td>Crime, Thriller</td>
      <td>7.7</td>
      <td>Danny Ocean and his ten accomplices plan to ro...</td>
      <td>74.00000</td>
      <td>Steven Soderbergh</td>
      <td>George Clooney</td>
      <td>Brad Pitt</td>
      <td>Julia Roberts</td>
      <td>Matt Damon</td>
      <td>516372</td>
      <td>183417150</td>
    </tr>
    <tr>
      <th>796</th>
      <td>Vampire Hunter D: Bloodlust</td>
      <td>2000</td>
      <td>U</td>
      <td>103</td>
      <td>Animation, Action, Fantasy</td>
      <td>7.7</td>
      <td>When a girl is abducted by a vampire, a legend...</td>
      <td>62.00000</td>
      <td>Yoshiaki Kawajiri</td>
      <td>Andrew Philpot</td>
      <td>John Rafter Lee</td>
      <td>Pamela Adlon</td>
      <td>Wendee Lee</td>
      <td>29210</td>
      <td>151086</td>
    </tr>
    <tr>
      <th>797</th>
      <td>O Brother, Where Art Thou?</td>
      <td>2000</td>
      <td>U</td>
      <td>107</td>
      <td>Adventure, Comedy, Crime</td>
      <td>7.7</td>
      <td>In the deep south during the 1930s, three esca...</td>
      <td>69.00000</td>
      <td>Joel Coen</td>
      <td>Ethan Coen</td>
      <td>George Clooney</td>
      <td>John Turturro</td>
      <td>Tim Blake Nelson</td>
      <td>286742</td>
      <td>45512588</td>
    </tr>
    <tr>
      <th>798</th>
      <td>Interstate 60: Episodes of the Road</td>
      <td>2002</td>
      <td>R</td>
      <td>116</td>
      <td>Adventure, Comedy, Drama</td>
      <td>7.7</td>
      <td>Neal Oliver, a very confused young man and an ...</td>
      <td>77.97153</td>
      <td>Bob Gale</td>
      <td>James Marsden</td>
      <td>Gary Oldman</td>
      <td>Kurt Russell</td>
      <td>Matthew Edison</td>
      <td>29999</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>799</th>
      <td>South Park: Bigger, Longer &amp; Uncut</td>
      <td>1999</td>
      <td>A</td>
      <td>81</td>
      <td>Animation, Comedy, Fantasy</td>
      <td>7.7</td>
      <td>When Stan Marsh and his friends go see an R-ra...</td>
      <td>73.00000</td>
      <td>Trey Parker</td>
      <td>Trey Parker</td>
      <td>Matt Stone</td>
      <td>Mary Kay Bergman</td>
      <td>Isaac Hayes</td>
      <td>192112</td>
      <td>52037603</td>
    </tr>
    <tr>
      <th>800</th>
      <td>Office Space</td>
      <td>1999</td>
      <td>R</td>
      <td>89</td>
      <td>Comedy</td>
      <td>7.7</td>
      <td>Three company workers who hate their jobs deci...</td>
      <td>68.00000</td>
      <td>Mike Judge</td>
      <td>Ron Livingston</td>
      <td>Jennifer Aniston</td>
      <td>David Herman</td>
      <td>Ajay Naidu</td>
      <td>241575</td>
      <td>10824921</td>
    </tr>
    <tr>
      <th>801</th>
      <td>Happiness</td>
      <td>1998</td>
      <td>Unknown</td>
      <td>134</td>
      <td>Comedy, Drama</td>
      <td>7.7</td>
      <td>The lives of several individuals intertwine as...</td>
      <td>81.00000</td>
      <td>Todd Solondz</td>
      <td>Jane Adams</td>
      <td>Jon Lovitz</td>
      <td>Philip Seymour Hoffman</td>
      <td>Dylan Baker</td>
      <td>66408</td>
      <td>2807390</td>
    </tr>
    <tr>
      <th>802</th>
      <td>Training Day</td>
      <td>2001</td>
      <td>A</td>
      <td>122</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.7</td>
      <td>A rookie cop spends his first day as a Los Ang...</td>
      <td>69.00000</td>
      <td>Antoine Fuqua</td>
      <td>Denzel Washington</td>
      <td>Ethan Hawke</td>
      <td>Scott Glenn</td>
      <td>Tom Berenger</td>
      <td>390247</td>
      <td>76631907</td>
    </tr>
    <tr>
      <th>803</th>
      <td>Rushmore</td>
      <td>1998</td>
      <td>UA</td>
      <td>93</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>The extracurricular king of Rushmore Preparato...</td>
      <td>86.00000</td>
      <td>Wes Anderson</td>
      <td>Jason Schwartzman</td>
      <td>Bill Murray</td>
      <td>Olivia Williams</td>
      <td>Seymour Cassel</td>
      <td>169229</td>
      <td>17105219</td>
    </tr>
    <tr>
      <th>804</th>
      <td>Abre los ojos</td>
      <td>1997</td>
      <td>U</td>
      <td>119</td>
      <td>Drama, Mystery, Sci-Fi</td>
      <td>7.7</td>
      <td>A very handsome man finds the love of his life...</td>
      <td>77.97153</td>
      <td>Alejandro Amenábar</td>
      <td>Eduardo Noriega</td>
      <td>Penélope Cruz</td>
      <td>Chete Lera</td>
      <td>Fele Martínez</td>
      <td>64082</td>
      <td>368234</td>
    </tr>
    <tr>
      <th>805</th>
      <td>Being John Malkovich</td>
      <td>1999</td>
      <td>R</td>
      <td>113</td>
      <td>Comedy, Drama, Fantasy</td>
      <td>7.7</td>
      <td>A puppeteer discovers a portal that leads lite...</td>
      <td>90.00000</td>
      <td>Spike Jonze</td>
      <td>John Cusack</td>
      <td>Cameron Diaz</td>
      <td>Catherine Keener</td>
      <td>John Malkovich</td>
      <td>312542</td>
      <td>22858926</td>
    </tr>
    <tr>
      <th>806</th>
      <td>As Good as It Gets</td>
      <td>1997</td>
      <td>A</td>
      <td>139</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>A single mother and waitress, a misanthropic a...</td>
      <td>67.00000</td>
      <td>James L. Brooks</td>
      <td>Jack Nicholson</td>
      <td>Helen Hunt</td>
      <td>Greg Kinnear</td>
      <td>Cuba Gooding Jr.</td>
      <td>275755</td>
      <td>148478011</td>
    </tr>
    <tr>
      <th>807</th>
      <td>The Fifth Element</td>
      <td>1997</td>
      <td>UA</td>
      <td>126</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.7</td>
      <td>In the colorful future, a cab driver unwitting...</td>
      <td>52.00000</td>
      <td>Luc Besson</td>
      <td>Bruce Willis</td>
      <td>Milla Jovovich</td>
      <td>Gary Oldman</td>
      <td>Ian Holm</td>
      <td>434125</td>
      <td>63540020</td>
    </tr>
    <tr>
      <th>808</th>
      <td>Le dîner de cons</td>
      <td>1998</td>
      <td>PG-13</td>
      <td>80</td>
      <td>Comedy</td>
      <td>7.7</td>
      <td>A few friends have a weekly fools' dinner, whe...</td>
      <td>73.00000</td>
      <td>Francis Veber</td>
      <td>Thierry Lhermitte</td>
      <td>Jacques Villeret</td>
      <td>Francis Huster</td>
      <td>Daniel Prévost</td>
      <td>37424</td>
      <td>4065116</td>
    </tr>
    <tr>
      <th>809</th>
      <td>Donnie Brasco</td>
      <td>1997</td>
      <td>A</td>
      <td>127</td>
      <td>Biography, Crime, Drama</td>
      <td>7.7</td>
      <td>An FBI undercover agent infiltrates the mob an...</td>
      <td>76.00000</td>
      <td>Mike Newell</td>
      <td>Al Pacino</td>
      <td>Johnny Depp</td>
      <td>Michael Madsen</td>
      <td>Bruno Kirby</td>
      <td>279318</td>
      <td>41909762</td>
    </tr>
    <tr>
      <th>810</th>
      <td>Shine</td>
      <td>1996</td>
      <td>U</td>
      <td>105</td>
      <td>Biography, Drama, Music</td>
      <td>7.7</td>
      <td>Pianist David Helfgott, driven by his father a...</td>
      <td>87.00000</td>
      <td>Scott Hicks</td>
      <td>Geoffrey Rush</td>
      <td>Armin Mueller-Stahl</td>
      <td>Justin Braine</td>
      <td>Sonia Todd</td>
      <td>51350</td>
      <td>35811509</td>
    </tr>
    <tr>
      <th>811</th>
      <td>Primal Fear</td>
      <td>1996</td>
      <td>A</td>
      <td>129</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.7</td>
      <td>An altar boy is accused of murdering a priest,...</td>
      <td>47.00000</td>
      <td>Gregory Hoblit</td>
      <td>Richard Gere</td>
      <td>Laura Linney</td>
      <td>Edward Norton</td>
      <td>John Mahoney</td>
      <td>189716</td>
      <td>56116183</td>
    </tr>
    <tr>
      <th>812</th>
      <td>Hamlet</td>
      <td>1996</td>
      <td>PG-13</td>
      <td>242</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>Hamlet, Prince of Denmark, returns home to fin...</td>
      <td>77.97153</td>
      <td>Kenneth Branagh</td>
      <td>Kenneth Branagh</td>
      <td>Julie Christie</td>
      <td>Derek Jacobi</td>
      <td>Kate Winslet</td>
      <td>35991</td>
      <td>4414535</td>
    </tr>
    <tr>
      <th>813</th>
      <td>A Little Princess</td>
      <td>1995</td>
      <td>U</td>
      <td>97</td>
      <td>Drama, Family, Fantasy</td>
      <td>7.7</td>
      <td>A young girl is relegated to servitude at a bo...</td>
      <td>83.00000</td>
      <td>Alfonso Cuarón</td>
      <td>Liesel Matthews</td>
      <td>Eleanor Bron</td>
      <td>Liam Cunningham</td>
      <td>Rusty Schwimmer</td>
      <td>32236</td>
      <td>10019307</td>
    </tr>
    <tr>
      <th>814</th>
      <td>Do lok tin si</td>
      <td>1995</td>
      <td>UA</td>
      <td>99</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.7</td>
      <td>This Hong Kong-set crime drama follows the liv...</td>
      <td>71.00000</td>
      <td>Kar-Wai Wong</td>
      <td>Leon Lai</td>
      <td>Michelle Reis</td>
      <td>Takeshi Kaneshiro</td>
      <td>Charlie Yeung</td>
      <td>26429</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>815</th>
      <td>Il postino</td>
      <td>1994</td>
      <td>U</td>
      <td>108</td>
      <td>Biography, Comedy, Drama</td>
      <td>7.7</td>
      <td>A simple Italian postman learns to love poetry...</td>
      <td>81.00000</td>
      <td>Michael Radford</td>
      <td>Massimo Troisi</td>
      <td>Massimo Troisi</td>
      <td>Philippe Noiret</td>
      <td>Maria Grazia Cucinotta</td>
      <td>33600</td>
      <td>21848932</td>
    </tr>
    <tr>
      <th>816</th>
      <td>Clerks</td>
      <td>1994</td>
      <td>R</td>
      <td>92</td>
      <td>Comedy</td>
      <td>7.7</td>
      <td>A day in the lives of two convenience clerks n...</td>
      <td>70.00000</td>
      <td>Kevin Smith</td>
      <td>Brian O'Halloran</td>
      <td>Jeff Anderson</td>
      <td>Marilyn Ghigliotti</td>
      <td>Lisa Spoonauer</td>
      <td>211450</td>
      <td>3151130</td>
    </tr>
    <tr>
      <th>817</th>
      <td>Short Cuts</td>
      <td>1993</td>
      <td>R</td>
      <td>188</td>
      <td>Comedy, Drama</td>
      <td>7.7</td>
      <td>The day-to-day lives of several suburban Los A...</td>
      <td>79.00000</td>
      <td>Robert Altman</td>
      <td>Andie MacDowell</td>
      <td>Julianne Moore</td>
      <td>Tim Robbins</td>
      <td>Bruce Davison</td>
      <td>42275</td>
      <td>6110979</td>
    </tr>
    <tr>
      <th>818</th>
      <td>Philadelphia</td>
      <td>1993</td>
      <td>UA</td>
      <td>125</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>When a man with HIV is fired by his law firm b...</td>
      <td>66.00000</td>
      <td>Jonathan Demme</td>
      <td>Tom Hanks</td>
      <td>Denzel Washington</td>
      <td>Roberta Maxwell</td>
      <td>Buzz Kilman</td>
      <td>224169</td>
      <td>77324422</td>
    </tr>
    <tr>
      <th>819</th>
      <td>The Muppet Christmas Carol</td>
      <td>1992</td>
      <td>G</td>
      <td>85</td>
      <td>Comedy, Drama, Family</td>
      <td>7.7</td>
      <td>The Muppet characters tell their version of th...</td>
      <td>64.00000</td>
      <td>Brian Henson</td>
      <td>Michael Caine</td>
      <td>Kermit the Frog</td>
      <td>Dave Goelz</td>
      <td>Miss Piggy</td>
      <td>50298</td>
      <td>27281507</td>
    </tr>
    <tr>
      <th>820</th>
      <td>Malcolm X</td>
      <td>1992</td>
      <td>U</td>
      <td>202</td>
      <td>Biography, Drama, History</td>
      <td>7.7</td>
      <td>Biographical epic of the controversial and inf...</td>
      <td>73.00000</td>
      <td>Spike Lee</td>
      <td>Denzel Washington</td>
      <td>Angela Bassett</td>
      <td>Delroy Lindo</td>
      <td>Spike Lee</td>
      <td>85819</td>
      <td>48169908</td>
    </tr>
    <tr>
      <th>821</th>
      <td>The Last of the Mohicans</td>
      <td>1992</td>
      <td>UA</td>
      <td>112</td>
      <td>Action, Adventure, Drama</td>
      <td>7.7</td>
      <td>Three trappers protect the daughters of a Brit...</td>
      <td>76.00000</td>
      <td>Michael Mann</td>
      <td>Daniel Day-Lewis</td>
      <td>Madeleine Stowe</td>
      <td>Russell Means</td>
      <td>Eric Schweig</td>
      <td>150409</td>
      <td>75505856</td>
    </tr>
    <tr>
      <th>822</th>
      <td>Kurenai no buta</td>
      <td>1992</td>
      <td>U</td>
      <td>94</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.7</td>
      <td>In 1930s Italy, a veteran World War I pilot is...</td>
      <td>83.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Shûichirô Moriyama</td>
      <td>Tokiko Katô</td>
      <td>Bunshi Katsura Vi</td>
      <td>Tsunehiko Kamijô</td>
      <td>77798</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>823</th>
      <td>Glengarry Glen Ross</td>
      <td>1992</td>
      <td>R</td>
      <td>100</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.7</td>
      <td>An examination of the machinations behind the ...</td>
      <td>82.00000</td>
      <td>James Foley</td>
      <td>Al Pacino</td>
      <td>Jack Lemmon</td>
      <td>Alec Baldwin</td>
      <td>Alan Arkin</td>
      <td>95826</td>
      <td>10725228</td>
    </tr>
    <tr>
      <th>824</th>
      <td>A Few Good Men</td>
      <td>1992</td>
      <td>U</td>
      <td>138</td>
      <td>Drama, Thriller</td>
      <td>7.7</td>
      <td>Military lawyer Lieutenant Daniel Kaffee defen...</td>
      <td>62.00000</td>
      <td>Rob Reiner</td>
      <td>Tom Cruise</td>
      <td>Jack Nicholson</td>
      <td>Demi Moore</td>
      <td>Kevin Bacon</td>
      <td>235388</td>
      <td>141340178</td>
    </tr>
    <tr>
      <th>825</th>
      <td>Fried Green Tomatoes</td>
      <td>1991</td>
      <td>PG-13</td>
      <td>130</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>A housewife who is unhappy with her life befri...</td>
      <td>64.00000</td>
      <td>Jon Avnet</td>
      <td>Kathy Bates</td>
      <td>Jessica Tandy</td>
      <td>Mary Stuart Masterson</td>
      <td>Mary-Louise Parker</td>
      <td>66941</td>
      <td>82418501</td>
    </tr>
    <tr>
      <th>826</th>
      <td>Barton Fink</td>
      <td>1991</td>
      <td>U</td>
      <td>116</td>
      <td>Comedy, Drama, Thriller</td>
      <td>7.7</td>
      <td>A renowned New York playwright is enticed to C...</td>
      <td>69.00000</td>
      <td>Joel Coen</td>
      <td>Ethan Coen</td>
      <td>John Turturro</td>
      <td>John Goodman</td>
      <td>Judy Davis</td>
      <td>113240</td>
      <td>6153939</td>
    </tr>
    <tr>
      <th>827</th>
      <td>Miller's Crossing</td>
      <td>1990</td>
      <td>R</td>
      <td>115</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.7</td>
      <td>Tom Reagan, an advisor to a Prohibition-era cr...</td>
      <td>66.00000</td>
      <td>Joel Coen</td>
      <td>Ethan Coen</td>
      <td>Gabriel Byrne</td>
      <td>Albert Finney</td>
      <td>John Turturro</td>
      <td>125822</td>
      <td>5080409</td>
    </tr>
    <tr>
      <th>828</th>
      <td>Who Framed Roger Rabbit</td>
      <td>1988</td>
      <td>U</td>
      <td>104</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.7</td>
      <td>A toon-hating detective is a cartoon rabbit's ...</td>
      <td>83.00000</td>
      <td>Robert Zemeckis</td>
      <td>Bob Hoskins</td>
      <td>Christopher Lloyd</td>
      <td>Joanna Cassidy</td>
      <td>Charles Fleischer</td>
      <td>182009</td>
      <td>156452370</td>
    </tr>
    <tr>
      <th>829</th>
      <td>Spoorloos</td>
      <td>1988</td>
      <td>Unknown</td>
      <td>107</td>
      <td>Mystery, Thriller</td>
      <td>7.7</td>
      <td>Rex and Saskia, a young couple in love, are on...</td>
      <td>77.97153</td>
      <td>George Sluizer</td>
      <td>Bernard-Pierre Donnadieu</td>
      <td>Gene Bervoets</td>
      <td>Johanna ter Steege</td>
      <td>Gwen Eckhaus</td>
      <td>33982</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>830</th>
      <td>Withnail &amp; I</td>
      <td>1987</td>
      <td>R</td>
      <td>107</td>
      <td>Comedy, Drama</td>
      <td>7.7</td>
      <td>In 1969, two substance-abusing, unemployed act...</td>
      <td>84.00000</td>
      <td>Bruce Robinson</td>
      <td>Richard E. Grant</td>
      <td>Paul McGann</td>
      <td>Richard Griffiths</td>
      <td>Ralph Brown</td>
      <td>40396</td>
      <td>1544889</td>
    </tr>
    <tr>
      <th>831</th>
      <td>The Last Emperor</td>
      <td>1987</td>
      <td>U</td>
      <td>163</td>
      <td>Biography, Drama, History</td>
      <td>7.7</td>
      <td>The story of the final Emperor of China.</td>
      <td>76.00000</td>
      <td>Bernardo Bertolucci</td>
      <td>John Lone</td>
      <td>Joan Chen</td>
      <td>Peter O'Toole</td>
      <td>Ruocheng Ying</td>
      <td>94326</td>
      <td>43984230</td>
    </tr>
    <tr>
      <th>832</th>
      <td>Empire of the Sun</td>
      <td>1987</td>
      <td>U</td>
      <td>153</td>
      <td>Action, Drama, History</td>
      <td>7.7</td>
      <td>A young English boy struggles to survive under...</td>
      <td>62.00000</td>
      <td>Steven Spielberg</td>
      <td>Christian Bale</td>
      <td>John Malkovich</td>
      <td>Miranda Richardson</td>
      <td>Nigel Havers</td>
      <td>115677</td>
      <td>22238696</td>
    </tr>
    <tr>
      <th>833</th>
      <td>Der Name der Rose</td>
      <td>1986</td>
      <td>R</td>
      <td>130</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.7</td>
      <td>An intellectually nonconformist friar investig...</td>
      <td>54.00000</td>
      <td>Jean-Jacques Annaud</td>
      <td>Sean Connery</td>
      <td>Christian Slater</td>
      <td>Helmut Qualtinger</td>
      <td>Elya Baskin</td>
      <td>102031</td>
      <td>7153487</td>
    </tr>
    <tr>
      <th>834</th>
      <td>Blue Velvet</td>
      <td>1986</td>
      <td>A</td>
      <td>120</td>
      <td>Drama, Mystery, Thriller</td>
      <td>7.7</td>
      <td>The discovery of a severed human ear found in ...</td>
      <td>76.00000</td>
      <td>David Lynch</td>
      <td>Isabella Rossellini</td>
      <td>Kyle MacLachlan</td>
      <td>Dennis Hopper</td>
      <td>Laura Dern</td>
      <td>181285</td>
      <td>8551228</td>
    </tr>
    <tr>
      <th>835</th>
      <td>The Purple Rose of Cairo</td>
      <td>1985</td>
      <td>U</td>
      <td>82</td>
      <td>Comedy, Fantasy, Romance</td>
      <td>7.7</td>
      <td>In New Jersey in 1935, a movie character walks...</td>
      <td>75.00000</td>
      <td>Woody Allen</td>
      <td>Mia Farrow</td>
      <td>Jeff Daniels</td>
      <td>Danny Aiello</td>
      <td>Irving Metzman</td>
      <td>47102</td>
      <td>10631333</td>
    </tr>
    <tr>
      <th>836</th>
      <td>After Hours</td>
      <td>1985</td>
      <td>UA</td>
      <td>97</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.7</td>
      <td>An ordinary word processor has the worst night...</td>
      <td>90.00000</td>
      <td>Martin Scorsese</td>
      <td>Griffin Dunne</td>
      <td>Rosanna Arquette</td>
      <td>Verna Bloom</td>
      <td>Tommy Chong</td>
      <td>59635</td>
      <td>10600000</td>
    </tr>
    <tr>
      <th>837</th>
      <td>Zelig</td>
      <td>1983</td>
      <td>PG</td>
      <td>79</td>
      <td>Comedy</td>
      <td>7.7</td>
      <td>"Documentary" about a man who can look and act...</td>
      <td>77.97153</td>
      <td>Woody Allen</td>
      <td>Woody Allen</td>
      <td>Mia Farrow</td>
      <td>Patrick Horgan</td>
      <td>John Buckwalter</td>
      <td>39881</td>
      <td>11798616</td>
    </tr>
    <tr>
      <th>838</th>
      <td>The Verdict</td>
      <td>1982</td>
      <td>U</td>
      <td>129</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>A lawyer sees the chance to salvage his career...</td>
      <td>77.00000</td>
      <td>Sidney Lumet</td>
      <td>Paul Newman</td>
      <td>Charlotte Rampling</td>
      <td>Jack Warden</td>
      <td>James Mason</td>
      <td>36096</td>
      <td>54000000</td>
    </tr>
    <tr>
      <th>839</th>
      <td>Star Trek II: The Wrath of Khan</td>
      <td>1982</td>
      <td>U</td>
      <td>113</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.7</td>
      <td>With the assistance of the Enterprise crew, Ad...</td>
      <td>67.00000</td>
      <td>Nicholas Meyer</td>
      <td>William Shatner</td>
      <td>Leonard Nimoy</td>
      <td>DeForest Kelley</td>
      <td>James Doohan</td>
      <td>112704</td>
      <td>78912963</td>
    </tr>
    <tr>
      <th>840</th>
      <td>First Blood</td>
      <td>1982</td>
      <td>A</td>
      <td>93</td>
      <td>Action, Adventure</td>
      <td>7.7</td>
      <td>A veteran Green Beret is forced by a cruel She...</td>
      <td>61.00000</td>
      <td>Ted Kotcheff</td>
      <td>Sylvester Stallone</td>
      <td>Brian Dennehy</td>
      <td>Richard Crenna</td>
      <td>Bill McKinney</td>
      <td>226541</td>
      <td>47212904</td>
    </tr>
    <tr>
      <th>841</th>
      <td>Ordinary People</td>
      <td>1980</td>
      <td>U</td>
      <td>124</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>The accidental death of the older son of an af...</td>
      <td>86.00000</td>
      <td>Robert Redford</td>
      <td>Donald Sutherland</td>
      <td>Mary Tyler Moore</td>
      <td>Judd Hirsch</td>
      <td>Timothy Hutton</td>
      <td>47099</td>
      <td>54800000</td>
    </tr>
    <tr>
      <th>842</th>
      <td>Airplane!</td>
      <td>1980</td>
      <td>U</td>
      <td>88</td>
      <td>Comedy</td>
      <td>7.7</td>
      <td>A man afraid to fly must ensure that a plane l...</td>
      <td>78.00000</td>
      <td>Jim Abrahams</td>
      <td>David Zucker</td>
      <td>Jerry Zucker</td>
      <td>Robert Hays</td>
      <td>Julie Hagerty</td>
      <td>214882</td>
      <td>83400000</td>
    </tr>
    <tr>
      <th>843</th>
      <td>Rupan sansei: Kariosutoro no shiro</td>
      <td>1979</td>
      <td>U</td>
      <td>100</td>
      <td>Animation, Adventure, Family</td>
      <td>7.7</td>
      <td>A dashing thief, his gang of desperadoes and a...</td>
      <td>71.00000</td>
      <td>Hayao Miyazaki</td>
      <td>Yasuo Yamada</td>
      <td>Eiko Masuyama</td>
      <td>Kiyoshi Kobayashi</td>
      <td>Makio Inoue</td>
      <td>27014</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>844</th>
      <td>Halloween</td>
      <td>1978</td>
      <td>A</td>
      <td>91</td>
      <td>Horror, Thriller</td>
      <td>7.7</td>
      <td>Fifteen years after murdering his sister on Ha...</td>
      <td>87.00000</td>
      <td>John Carpenter</td>
      <td>Donald Pleasence</td>
      <td>Jamie Lee Curtis</td>
      <td>Tony Moran</td>
      <td>Nancy Kyes</td>
      <td>233106</td>
      <td>47000000</td>
    </tr>
    <tr>
      <th>845</th>
      <td>Le locataire</td>
      <td>1976</td>
      <td>R</td>
      <td>126</td>
      <td>Drama, Thriller</td>
      <td>7.7</td>
      <td>A bureaucrat rents a Paris apartment where he ...</td>
      <td>71.00000</td>
      <td>Roman Polanski</td>
      <td>Roman Polanski</td>
      <td>Isabelle Adjani</td>
      <td>Melvyn Douglas</td>
      <td>Jo Van Fleet</td>
      <td>39889</td>
      <td>1924733</td>
    </tr>
    <tr>
      <th>846</th>
      <td>Love and Death</td>
      <td>1975</td>
      <td>PG</td>
      <td>85</td>
      <td>Comedy, War</td>
      <td>7.7</td>
      <td>In czarist Russia, a neurotic soldier and his ...</td>
      <td>89.00000</td>
      <td>Woody Allen</td>
      <td>Woody Allen</td>
      <td>Diane Keaton</td>
      <td>Georges Adet</td>
      <td>Frank Adu</td>
      <td>36037</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>847</th>
      <td>The Taking of Pelham One Two Three</td>
      <td>1974</td>
      <td>U</td>
      <td>104</td>
      <td>Action, Crime, Thriller</td>
      <td>7.7</td>
      <td>In New York, armed men hijack a subway car and...</td>
      <td>68.00000</td>
      <td>Joseph Sargent</td>
      <td>Walter Matthau</td>
      <td>Robert Shaw</td>
      <td>Martin Balsam</td>
      <td>Hector Elizondo</td>
      <td>26729</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>848</th>
      <td>Blazing Saddles</td>
      <td>1974</td>
      <td>A</td>
      <td>93</td>
      <td>Comedy, Western</td>
      <td>7.7</td>
      <td>In order to ruin a western town, a corrupt pol...</td>
      <td>73.00000</td>
      <td>Mel Brooks</td>
      <td>Cleavon Little</td>
      <td>Gene Wilder</td>
      <td>Slim Pickens</td>
      <td>Harvey Korman</td>
      <td>125993</td>
      <td>119500000</td>
    </tr>
    <tr>
      <th>849</th>
      <td>Serpico</td>
      <td>1973</td>
      <td>A</td>
      <td>130</td>
      <td>Biography, Crime, Drama</td>
      <td>7.7</td>
      <td>An honest New York cop named Frank Serpico blo...</td>
      <td>87.00000</td>
      <td>Sidney Lumet</td>
      <td>Al Pacino</td>
      <td>John Randolph</td>
      <td>Jack Kehoe</td>
      <td>Biff McGuire</td>
      <td>109941</td>
      <td>29800000</td>
    </tr>
    <tr>
      <th>850</th>
      <td>Enter the Dragon</td>
      <td>1973</td>
      <td>A</td>
      <td>102</td>
      <td>Action, Crime, Drama</td>
      <td>7.7</td>
      <td>A secret agent comes to an opium lord's island...</td>
      <td>83.00000</td>
      <td>Robert Clouse</td>
      <td>Bruce Lee</td>
      <td>John Saxon</td>
      <td>Jim Kelly</td>
      <td>Ahna Capri</td>
      <td>96561</td>
      <td>25000000</td>
    </tr>
    <tr>
      <th>851</th>
      <td>Deliverance</td>
      <td>1972</td>
      <td>U</td>
      <td>109</td>
      <td>Adventure, Drama, Thriller</td>
      <td>7.7</td>
      <td>Intent on seeing the Cahulawassee River before...</td>
      <td>80.00000</td>
      <td>John Boorman</td>
      <td>Jon Voight</td>
      <td>Burt Reynolds</td>
      <td>Ned Beatty</td>
      <td>Ronny Cox</td>
      <td>98740</td>
      <td>7056013</td>
    </tr>
    <tr>
      <th>852</th>
      <td>The French Connection</td>
      <td>1971</td>
      <td>A</td>
      <td>104</td>
      <td>Action, Crime, Drama</td>
      <td>7.7</td>
      <td>A pair of NYC cops in the Narcotics Bureau stu...</td>
      <td>94.00000</td>
      <td>William Friedkin</td>
      <td>Gene Hackman</td>
      <td>Roy Scheider</td>
      <td>Fernando Rey</td>
      <td>Tony Lo Bianco</td>
      <td>110075</td>
      <td>15630710</td>
    </tr>
    <tr>
      <th>853</th>
      <td>Dirty Harry</td>
      <td>1971</td>
      <td>A</td>
      <td>102</td>
      <td>Action, Crime, Thriller</td>
      <td>7.7</td>
      <td>When a madman calling himself "the Scorpio Kil...</td>
      <td>90.00000</td>
      <td>Don Siegel</td>
      <td>Clint Eastwood</td>
      <td>Andrew Robinson</td>
      <td>Harry Guardino</td>
      <td>Reni Santoni</td>
      <td>143292</td>
      <td>35900000</td>
    </tr>
    <tr>
      <th>854</th>
      <td>Where Eagles Dare</td>
      <td>1968</td>
      <td>U</td>
      <td>158</td>
      <td>Action, Adventure, War</td>
      <td>7.7</td>
      <td>Allied agents stage a daring raid on a castle ...</td>
      <td>63.00000</td>
      <td>Brian G. Hutton</td>
      <td>Richard Burton</td>
      <td>Clint Eastwood</td>
      <td>Mary Ure</td>
      <td>Patrick Wymark</td>
      <td>51913</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>855</th>
      <td>The Odd Couple</td>
      <td>1968</td>
      <td>G</td>
      <td>105</td>
      <td>Comedy</td>
      <td>7.7</td>
      <td>Two friends try sharing an apartment, but thei...</td>
      <td>86.00000</td>
      <td>Gene Saks</td>
      <td>Jack Lemmon</td>
      <td>Walter Matthau</td>
      <td>John Fiedler</td>
      <td>Herb Edelman</td>
      <td>31572</td>
      <td>44527234</td>
    </tr>
    <tr>
      <th>856</th>
      <td>The Dirty Dozen</td>
      <td>1967</td>
      <td>Unknown</td>
      <td>150</td>
      <td>Action, Adventure, War</td>
      <td>7.7</td>
      <td>During World War II, a rebellious U.S. Army Ma...</td>
      <td>73.00000</td>
      <td>Robert Aldrich</td>
      <td>Lee Marvin</td>
      <td>Ernest Borgnine</td>
      <td>Charles Bronson</td>
      <td>John Cassavetes</td>
      <td>67183</td>
      <td>45300000</td>
    </tr>
    <tr>
      <th>857</th>
      <td>Belle de jour</td>
      <td>1967</td>
      <td>A</td>
      <td>100</td>
      <td>Drama, Romance</td>
      <td>7.7</td>
      <td>A frigid young housewife decides to spend her ...</td>
      <td>77.97153</td>
      <td>Luis Buñuel</td>
      <td>Catherine Deneuve</td>
      <td>Jean Sorel</td>
      <td>Michel Piccoli</td>
      <td>Geneviève Page</td>
      <td>40274</td>
      <td>26331</td>
    </tr>
    <tr>
      <th>858</th>
      <td>A Man for All Seasons</td>
      <td>1966</td>
      <td>U</td>
      <td>120</td>
      <td>Biography, Drama, History</td>
      <td>7.7</td>
      <td>The story of Sir Thomas More, who stood up to ...</td>
      <td>72.00000</td>
      <td>Fred Zinnemann</td>
      <td>Paul Scofield</td>
      <td>Wendy Hiller</td>
      <td>Robert Shaw</td>
      <td>Leo McKern</td>
      <td>31222</td>
      <td>28350000</td>
    </tr>
    <tr>
      <th>859</th>
      <td>Repulsion</td>
      <td>1965</td>
      <td>Unknown</td>
      <td>105</td>
      <td>Drama, Horror, Thriller</td>
      <td>7.7</td>
      <td>A sex-repulsed woman who disapproves of her si...</td>
      <td>91.00000</td>
      <td>Roman Polanski</td>
      <td>Catherine Deneuve</td>
      <td>Ian Hendry</td>
      <td>John Fraser</td>
      <td>Yvonne Furneaux</td>
      <td>48883</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>860</th>
      <td>Zulu</td>
      <td>1964</td>
      <td>U</td>
      <td>138</td>
      <td>Drama, History, War</td>
      <td>7.7</td>
      <td>Outnumbered British soldiers do battle with Zu...</td>
      <td>77.00000</td>
      <td>Cy Endfield</td>
      <td>Stanley Baker</td>
      <td>Jack Hawkins</td>
      <td>Ulla Jacobsson</td>
      <td>James Booth</td>
      <td>35999</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>861</th>
      <td>Goldfinger</td>
      <td>1964</td>
      <td>A</td>
      <td>110</td>
      <td>Action, Adventure, Thriller</td>
      <td>7.7</td>
      <td>While investigating a gold magnate's smuggling...</td>
      <td>87.00000</td>
      <td>Guy Hamilton</td>
      <td>Sean Connery</td>
      <td>Gert Fröbe</td>
      <td>Honor Blackman</td>
      <td>Shirley Eaton</td>
      <td>174119</td>
      <td>51081062</td>
    </tr>
    <tr>
      <th>862</th>
      <td>The Birds</td>
      <td>1963</td>
      <td>A</td>
      <td>119</td>
      <td>Drama, Horror, Mystery</td>
      <td>7.7</td>
      <td>A wealthy San Francisco socialite pursues a po...</td>
      <td>90.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Rod Taylor</td>
      <td>Tippi Hedren</td>
      <td>Jessica Tandy</td>
      <td>Suzanne Pleshette</td>
      <td>171739</td>
      <td>11403529</td>
    </tr>
    <tr>
      <th>863</th>
      <td>Cape Fear</td>
      <td>1962</td>
      <td>Passed</td>
      <td>106</td>
      <td>Drama, Thriller</td>
      <td>7.7</td>
      <td>A lawyer's family is stalked by a man he once ...</td>
      <td>76.00000</td>
      <td>J. Lee Thompson</td>
      <td>Gregory Peck</td>
      <td>Robert Mitchum</td>
      <td>Polly Bergen</td>
      <td>Lori Martin</td>
      <td>26457</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>864</th>
      <td>Peeping Tom</td>
      <td>1960</td>
      <td>Unknown</td>
      <td>101</td>
      <td>Drama, Horror, Thriller</td>
      <td>7.7</td>
      <td>A young man murders women, using a movie camer...</td>
      <td>77.97153</td>
      <td>Michael Powell</td>
      <td>Karlheinz Böhm</td>
      <td>Anna Massey</td>
      <td>Moira Shearer</td>
      <td>Maxine Audley</td>
      <td>31354</td>
      <td>83957</td>
    </tr>
    <tr>
      <th>865</th>
      <td>The Magnificent Seven</td>
      <td>1960</td>
      <td>Approved</td>
      <td>128</td>
      <td>Action, Adventure, Western</td>
      <td>7.7</td>
      <td>Seven gunfighters are hired by Mexican peasant...</td>
      <td>74.00000</td>
      <td>John Sturges</td>
      <td>Yul Brynner</td>
      <td>Steve McQueen</td>
      <td>Charles Bronson</td>
      <td>Eli Wallach</td>
      <td>87719</td>
      <td>4905000</td>
    </tr>
    <tr>
      <th>866</th>
      <td>Les yeux sans visage</td>
      <td>1960</td>
      <td>Unknown</td>
      <td>90</td>
      <td>Drama, Horror</td>
      <td>7.7</td>
      <td>A surgeon causes an accident which leaves his ...</td>
      <td>90.00000</td>
      <td>Georges Franju</td>
      <td>Pierre Brasseur</td>
      <td>Alida Valli</td>
      <td>Juliette Mayniel</td>
      <td>Alexandre Rignault</td>
      <td>27620</td>
      <td>52709</td>
    </tr>
    <tr>
      <th>867</th>
      <td>Invasion of the Body Snatchers</td>
      <td>1956</td>
      <td>Approved</td>
      <td>80</td>
      <td>Drama, Horror, Sci-Fi</td>
      <td>7.7</td>
      <td>A small-town doctor learns that the population...</td>
      <td>92.00000</td>
      <td>Don Siegel</td>
      <td>Kevin McCarthy</td>
      <td>Dana Wynter</td>
      <td>Larry Gates</td>
      <td>King Donovan</td>
      <td>44839</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>868</th>
      <td>Rebel Without a Cause</td>
      <td>1955</td>
      <td>PG-13</td>
      <td>111</td>
      <td>Drama</td>
      <td>7.7</td>
      <td>A rebellious young man with a troubled past co...</td>
      <td>89.00000</td>
      <td>Nicholas Ray</td>
      <td>James Dean</td>
      <td>Natalie Wood</td>
      <td>Sal Mineo</td>
      <td>Jim Backus</td>
      <td>83363</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>869</th>
      <td>The Ladykillers</td>
      <td>1955</td>
      <td>Unknown</td>
      <td>91</td>
      <td>Comedy, Crime</td>
      <td>7.7</td>
      <td>Five oddball criminals planning a bank robbery...</td>
      <td>91.00000</td>
      <td>Alexander Mackendrick</td>
      <td>Alec Guinness</td>
      <td>Peter Sellers</td>
      <td>Cecil Parker</td>
      <td>Herbert Lom</td>
      <td>26464</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>870</th>
      <td>Sabrina</td>
      <td>1954</td>
      <td>Passed</td>
      <td>113</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>A playboy becomes interested in the daughter o...</td>
      <td>72.00000</td>
      <td>Billy Wilder</td>
      <td>Humphrey Bogart</td>
      <td>Audrey Hepburn</td>
      <td>William Holden</td>
      <td>Walter Hampden</td>
      <td>59415</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>871</th>
      <td>The Quiet Man</td>
      <td>1952</td>
      <td>Passed</td>
      <td>129</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.7</td>
      <td>A retired American boxer returns to the villag...</td>
      <td>77.97153</td>
      <td>John Ford</td>
      <td>John Wayne</td>
      <td>Maureen O'Hara</td>
      <td>Barry Fitzgerald</td>
      <td>Ward Bond</td>
      <td>34677</td>
      <td>10550000</td>
    </tr>
    <tr>
      <th>872</th>
      <td>The Day the Earth Stood Still</td>
      <td>1951</td>
      <td>U</td>
      <td>92</td>
      <td>Drama, Sci-Fi</td>
      <td>7.7</td>
      <td>An alien lands and tells the people of Earth t...</td>
      <td>77.97153</td>
      <td>Robert Wise</td>
      <td>Michael Rennie</td>
      <td>Patricia Neal</td>
      <td>Hugh Marlowe</td>
      <td>Sam Jaffe</td>
      <td>76315</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>873</th>
      <td>The African Queen</td>
      <td>1951</td>
      <td>PG</td>
      <td>105</td>
      <td>Adventure, Drama, Romance</td>
      <td>7.7</td>
      <td>In WWI Africa, a gin-swilling riverboat captai...</td>
      <td>91.00000</td>
      <td>John Huston</td>
      <td>Humphrey Bogart</td>
      <td>Katharine Hepburn</td>
      <td>Robert Morley</td>
      <td>Peter Bull</td>
      <td>71481</td>
      <td>536118</td>
    </tr>
    <tr>
      <th>874</th>
      <td>Gilda</td>
      <td>1946</td>
      <td>Approved</td>
      <td>110</td>
      <td>Drama, Film-Noir, Romance</td>
      <td>7.7</td>
      <td>A small-time gambler hired to work in a Buenos...</td>
      <td>77.97153</td>
      <td>Charles Vidor</td>
      <td>Rita Hayworth</td>
      <td>Glenn Ford</td>
      <td>George Macready</td>
      <td>Joseph Calleia</td>
      <td>27991</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>875</th>
      <td>Fantasia</td>
      <td>1940</td>
      <td>G</td>
      <td>125</td>
      <td>Animation, Family, Fantasy</td>
      <td>7.7</td>
      <td>A collection of animated interpretations of gr...</td>
      <td>96.00000</td>
      <td>James Algar</td>
      <td>Samuel Armstrong</td>
      <td>Ford Beebe Jr.</td>
      <td>Norman Ferguson</td>
      <td>David Hand</td>
      <td>88662</td>
      <td>76408097</td>
    </tr>
    <tr>
      <th>876</th>
      <td>The Invisible Man</td>
      <td>1933</td>
      <td>TV-PG</td>
      <td>71</td>
      <td>Horror, Sci-Fi</td>
      <td>7.7</td>
      <td>A scientist finds a way of becoming invisible,...</td>
      <td>87.00000</td>
      <td>James Whale</td>
      <td>Claude Rains</td>
      <td>Gloria Stuart</td>
      <td>William Harrigan</td>
      <td>Henry Travers</td>
      <td>30683</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>877</th>
      <td>Dark Waters</td>
      <td>2019</td>
      <td>PG-13</td>
      <td>126</td>
      <td>Biography, Drama, History</td>
      <td>7.6</td>
      <td>A corporate defense attorney takes on an envir...</td>
      <td>73.00000</td>
      <td>Todd Haynes</td>
      <td>Mark Ruffalo</td>
      <td>Anne Hathaway</td>
      <td>Tim Robbins</td>
      <td>Bill Pullman</td>
      <td>60408</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>878</th>
      <td>Searching</td>
      <td>2018</td>
      <td>U/A</td>
      <td>102</td>
      <td>Drama, Mystery, Thriller</td>
      <td>7.6</td>
      <td>After his teenage daughter goes missing, a des...</td>
      <td>71.00000</td>
      <td>Aneesh Chaganty</td>
      <td>John Cho</td>
      <td>Debra Messing</td>
      <td>Joseph Lee</td>
      <td>Michelle La</td>
      <td>140840</td>
      <td>26020957</td>
    </tr>
    <tr>
      <th>879</th>
      <td>Once Upon a Time... in Hollywood</td>
      <td>2019</td>
      <td>A</td>
      <td>161</td>
      <td>Comedy, Drama</td>
      <td>7.6</td>
      <td>A faded television actor and his stunt double ...</td>
      <td>83.00000</td>
      <td>Quentin Tarantino</td>
      <td>Leonardo DiCaprio</td>
      <td>Brad Pitt</td>
      <td>Margot Robbie</td>
      <td>Emile Hirsch</td>
      <td>551309</td>
      <td>142502728</td>
    </tr>
    <tr>
      <th>880</th>
      <td>Nelyubov</td>
      <td>2017</td>
      <td>R</td>
      <td>127</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>A couple going through a divorce must team up ...</td>
      <td>86.00000</td>
      <td>Andrey Zvyagintsev</td>
      <td>Maryana Spivak</td>
      <td>Aleksey Rozin</td>
      <td>Matvey Novikov</td>
      <td>Marina Vasileva</td>
      <td>29765</td>
      <td>566356</td>
    </tr>
    <tr>
      <th>881</th>
      <td>The Florida Project</td>
      <td>2017</td>
      <td>A</td>
      <td>111</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>Set over one summer, the film follows precocio...</td>
      <td>92.00000</td>
      <td>Sean Baker</td>
      <td>Brooklynn Prince</td>
      <td>Bria Vinaite</td>
      <td>Willem Dafoe</td>
      <td>Christopher Rivera</td>
      <td>95181</td>
      <td>5904366</td>
    </tr>
    <tr>
      <th>882</th>
      <td>Just Mercy</td>
      <td>2019</td>
      <td>A</td>
      <td>137</td>
      <td>Biography, Crime, Drama</td>
      <td>7.6</td>
      <td>World-renowned civil rights defense attorney B...</td>
      <td>68.00000</td>
      <td>Destin Daniel Cretton</td>
      <td>Michael B. Jordan</td>
      <td>Jamie Foxx</td>
      <td>Brie Larson</td>
      <td>Charlie Pye Jr.</td>
      <td>46739</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>883</th>
      <td>Gifted</td>
      <td>2017</td>
      <td>PG-13</td>
      <td>101</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>Frank, a single man raising his child prodigy ...</td>
      <td>60.00000</td>
      <td>Marc Webb</td>
      <td>Chris Evans</td>
      <td>Mckenna Grace</td>
      <td>Lindsay Duncan</td>
      <td>Octavia Spencer</td>
      <td>99643</td>
      <td>24801212</td>
    </tr>
    <tr>
      <th>884</th>
      <td>The Peanut Butter Falcon</td>
      <td>2019</td>
      <td>PG-13</td>
      <td>97</td>
      <td>Adventure, Comedy, Drama</td>
      <td>7.6</td>
      <td>Zak runs away from his care home to make his d...</td>
      <td>70.00000</td>
      <td>Tyler Nilson</td>
      <td>Michael Schwartz</td>
      <td>Zack Gottsagen</td>
      <td>Ann Owens</td>
      <td>Dakota Johnson</td>
      <td>66346</td>
      <td>13122642</td>
    </tr>
    <tr>
      <th>885</th>
      <td>Victoria</td>
      <td>2015</td>
      <td>Unknown</td>
      <td>138</td>
      <td>Crime, Drama, Romance</td>
      <td>7.6</td>
      <td>A young Spanish woman who has recently moved t...</td>
      <td>77.00000</td>
      <td>Sebastian Schipper</td>
      <td>Laia Costa</td>
      <td>Frederick Lau</td>
      <td>Franz Rogowski</td>
      <td>Burak Yigit</td>
      <td>52903</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>886</th>
      <td>Mustang</td>
      <td>2015</td>
      <td>PG-13</td>
      <td>97</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>When five orphan girls are seen innocently pla...</td>
      <td>83.00000</td>
      <td>Deniz Gamze Ergüven</td>
      <td>Günes Sensoy</td>
      <td>Doga Zeynep Doguslu</td>
      <td>Tugba Sunguroglu</td>
      <td>Elit Iscan</td>
      <td>35785</td>
      <td>845464</td>
    </tr>
    <tr>
      <th>887</th>
      <td>Guardians of the Galaxy Vol. 2</td>
      <td>2017</td>
      <td>UA</td>
      <td>136</td>
      <td>Action, Adventure, Comedy</td>
      <td>7.6</td>
      <td>The Guardians struggle to keep together as a t...</td>
      <td>67.00000</td>
      <td>James Gunn</td>
      <td>Chris Pratt</td>
      <td>Zoe Saldana</td>
      <td>Dave Bautista</td>
      <td>Vin Diesel</td>
      <td>569974</td>
      <td>389813101</td>
    </tr>
    <tr>
      <th>888</th>
      <td>Baby Driver</td>
      <td>2017</td>
      <td>UA</td>
      <td>113</td>
      <td>Action, Crime, Drama</td>
      <td>7.6</td>
      <td>After being coerced into working for a crime b...</td>
      <td>86.00000</td>
      <td>Edgar Wright</td>
      <td>Ansel Elgort</td>
      <td>Jon Bernthal</td>
      <td>Jon Hamm</td>
      <td>Eiza González</td>
      <td>439406</td>
      <td>107825862</td>
    </tr>
    <tr>
      <th>889</th>
      <td>Only the Brave</td>
      <td>2017</td>
      <td>UA</td>
      <td>134</td>
      <td>Action, Biography, Drama</td>
      <td>7.6</td>
      <td>Based on the true story of the Granite Mountai...</td>
      <td>72.00000</td>
      <td>Joseph Kosinski</td>
      <td>Josh Brolin</td>
      <td>Miles Teller</td>
      <td>Jeff Bridges</td>
      <td>Jennifer Connelly</td>
      <td>58371</td>
      <td>18340051</td>
    </tr>
    <tr>
      <th>890</th>
      <td>Bridge of Spies</td>
      <td>2015</td>
      <td>UA</td>
      <td>142</td>
      <td>Drama, History, Thriller</td>
      <td>7.6</td>
      <td>During the Cold War, an American lawyer is rec...</td>
      <td>81.00000</td>
      <td>Steven Spielberg</td>
      <td>Tom Hanks</td>
      <td>Mark Rylance</td>
      <td>Alan Alda</td>
      <td>Amy Ryan</td>
      <td>287659</td>
      <td>72313754</td>
    </tr>
    <tr>
      <th>891</th>
      <td>Incredibles 2</td>
      <td>2018</td>
      <td>UA</td>
      <td>118</td>
      <td>Animation, Action, Adventure</td>
      <td>7.6</td>
      <td>The Incredibles family takes on a new mission ...</td>
      <td>80.00000</td>
      <td>Brad Bird</td>
      <td>Craig T. Nelson</td>
      <td>Holly Hunter</td>
      <td>Sarah Vowell</td>
      <td>Huck Milner</td>
      <td>250057</td>
      <td>608581744</td>
    </tr>
    <tr>
      <th>892</th>
      <td>Moana</td>
      <td>2016</td>
      <td>U</td>
      <td>107</td>
      <td>Animation, Adventure, Comedy</td>
      <td>7.6</td>
      <td>In Ancient Polynesia, when a terrible curse in...</td>
      <td>81.00000</td>
      <td>Ron Clements</td>
      <td>John Musker</td>
      <td>Don Hall</td>
      <td>Chris Williams</td>
      <td>Auli'i Cravalho</td>
      <td>272784</td>
      <td>248757044</td>
    </tr>
    <tr>
      <th>893</th>
      <td>Sicario</td>
      <td>2015</td>
      <td>A</td>
      <td>121</td>
      <td>Action, Crime, Drama</td>
      <td>7.6</td>
      <td>An idealistic FBI agent is enlisted by a gover...</td>
      <td>82.00000</td>
      <td>Denis Villeneuve</td>
      <td>Emily Blunt</td>
      <td>Josh Brolin</td>
      <td>Benicio Del Toro</td>
      <td>Jon Bernthal</td>
      <td>371291</td>
      <td>46889293</td>
    </tr>
    <tr>
      <th>894</th>
      <td>Creed</td>
      <td>2015</td>
      <td>A</td>
      <td>133</td>
      <td>Drama, Sport</td>
      <td>7.6</td>
      <td>The former World Heavyweight Champion Rocky Ba...</td>
      <td>82.00000</td>
      <td>Ryan Coogler</td>
      <td>Michael B. Jordan</td>
      <td>Sylvester Stallone</td>
      <td>Tessa Thompson</td>
      <td>Phylicia Rashad</td>
      <td>247666</td>
      <td>109767581</td>
    </tr>
    <tr>
      <th>895</th>
      <td>Leviafan</td>
      <td>2014</td>
      <td>R</td>
      <td>140</td>
      <td>Crime, Drama</td>
      <td>7.6</td>
      <td>In a Russian coastal town, Kolya is forced to ...</td>
      <td>92.00000</td>
      <td>Andrey Zvyagintsev</td>
      <td>Aleksey Serebryakov</td>
      <td>Elena Lyadova</td>
      <td>Roman Madyanov</td>
      <td>Vladimir Vdovichenkov</td>
      <td>49397</td>
      <td>1092800</td>
    </tr>
    <tr>
      <th>896</th>
      <td>Hell or High Water</td>
      <td>2016</td>
      <td>R</td>
      <td>102</td>
      <td>Action, Crime, Drama</td>
      <td>7.6</td>
      <td>A divorced father and his ex-con older brother...</td>
      <td>88.00000</td>
      <td>David Mackenzie</td>
      <td>Chris Pine</td>
      <td>Ben Foster</td>
      <td>Jeff Bridges</td>
      <td>Gil Birmingham</td>
      <td>204175</td>
      <td>26862450</td>
    </tr>
    <tr>
      <th>897</th>
      <td>Philomena</td>
      <td>2013</td>
      <td>PG-13</td>
      <td>98</td>
      <td>Biography, Comedy, Drama</td>
      <td>7.6</td>
      <td>A world-weary political journalist picks up th...</td>
      <td>77.00000</td>
      <td>Stephen Frears</td>
      <td>Judi Dench</td>
      <td>Steve Coogan</td>
      <td>Sophie Kennedy Clark</td>
      <td>Mare Winningham</td>
      <td>94212</td>
      <td>37707719</td>
    </tr>
    <tr>
      <th>898</th>
      <td>Dawn of the Planet of the Apes</td>
      <td>2014</td>
      <td>UA</td>
      <td>130</td>
      <td>Action, Adventure, Drama</td>
      <td>7.6</td>
      <td>A growing nation of genetically evolved apes l...</td>
      <td>79.00000</td>
      <td>Matt Reeves</td>
      <td>Gary Oldman</td>
      <td>Keri Russell</td>
      <td>Andy Serkis</td>
      <td>Kodi Smit-McPhee</td>
      <td>411599</td>
      <td>208545589</td>
    </tr>
    <tr>
      <th>899</th>
      <td>El cuerpo</td>
      <td>2012</td>
      <td>Unknown</td>
      <td>112</td>
      <td>Mystery, Thriller</td>
      <td>7.6</td>
      <td>A detective searches for the body of a femme f...</td>
      <td>77.97153</td>
      <td>Oriol Paulo</td>
      <td>Jose Coronado</td>
      <td>Hugo Silva</td>
      <td>Belén Rueda</td>
      <td>Aura Garrido</td>
      <td>57549</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>900</th>
      <td>Serbuan maut</td>
      <td>2011</td>
      <td>A</td>
      <td>101</td>
      <td>Action, Thriller</td>
      <td>7.6</td>
      <td>A S.W.A.T. team becomes trapped in a tenement ...</td>
      <td>73.00000</td>
      <td>Gareth Evans</td>
      <td>Iko Uwais</td>
      <td>Ananda George</td>
      <td>Ray Sahetapy</td>
      <td>Donny Alamsyah</td>
      <td>190531</td>
      <td>4105123</td>
    </tr>
    <tr>
      <th>901</th>
      <td>End of Watch</td>
      <td>2012</td>
      <td>A</td>
      <td>109</td>
      <td>Action, Crime, Drama</td>
      <td>7.6</td>
      <td>Shot documentary-style, this film follows the ...</td>
      <td>68.00000</td>
      <td>David Ayer</td>
      <td>Jake Gyllenhaal</td>
      <td>Michael Peña</td>
      <td>Anna Kendrick</td>
      <td>America Ferrera</td>
      <td>228132</td>
      <td>41003371</td>
    </tr>
    <tr>
      <th>902</th>
      <td>Kari-gurashi no Arietti</td>
      <td>2010</td>
      <td>U</td>
      <td>94</td>
      <td>Animation, Adventure, Family</td>
      <td>7.6</td>
      <td>The Clock family are four-inch-tall people who...</td>
      <td>80.00000</td>
      <td>Hiromasa Yonebayashi</td>
      <td>Amy Poehler</td>
      <td>Mirai Shida</td>
      <td>Ryûnosuke Kamiki</td>
      <td>Tatsuya Fujiwara</td>
      <td>80939</td>
      <td>19202743</td>
    </tr>
    <tr>
      <th>903</th>
      <td>A Star Is Born</td>
      <td>2018</td>
      <td>UA</td>
      <td>136</td>
      <td>Drama, Music, Romance</td>
      <td>7.6</td>
      <td>A musician helps a young singer find fame as a...</td>
      <td>88.00000</td>
      <td>Bradley Cooper</td>
      <td>Lady Gaga</td>
      <td>Bradley Cooper</td>
      <td>Sam Elliott</td>
      <td>Greg Grunberg</td>
      <td>334312</td>
      <td>215288866</td>
    </tr>
    <tr>
      <th>904</th>
      <td>True Grit</td>
      <td>2010</td>
      <td>PG-13</td>
      <td>110</td>
      <td>Drama, Western</td>
      <td>7.6</td>
      <td>A stubborn teenager enlists the help of a toug...</td>
      <td>80.00000</td>
      <td>Ethan Coen</td>
      <td>Joel Coen</td>
      <td>Jeff Bridges</td>
      <td>Matt Damon</td>
      <td>Hailee Steinfeld</td>
      <td>311822</td>
      <td>171243005</td>
    </tr>
    <tr>
      <th>905</th>
      <td>Hævnen</td>
      <td>2010</td>
      <td>R</td>
      <td>118</td>
      <td>Drama, Romance</td>
      <td>7.6</td>
      <td>The lives of two Danish families cross each ot...</td>
      <td>65.00000</td>
      <td>Susanne Bier</td>
      <td>Mikael Persbrandt</td>
      <td>Trine Dyrholm</td>
      <td>Markus Rygaard</td>
      <td>Wil Johnson</td>
      <td>38491</td>
      <td>1008098</td>
    </tr>
    <tr>
      <th>906</th>
      <td>Despicable Me</td>
      <td>2010</td>
      <td>U</td>
      <td>95</td>
      <td>Animation, Comedy, Crime</td>
      <td>7.6</td>
      <td>When a criminal mastermind uses a trio of orph...</td>
      <td>72.00000</td>
      <td>Pierre Coffin</td>
      <td>Chris Renaud</td>
      <td>Steve Carell</td>
      <td>Jason Segel</td>
      <td>Russell Brand</td>
      <td>500851</td>
      <td>251513985</td>
    </tr>
    <tr>
      <th>907</th>
      <td>50/50</td>
      <td>2011</td>
      <td>R</td>
      <td>100</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.6</td>
      <td>Inspired by a true story, a comedy centered on...</td>
      <td>72.00000</td>
      <td>Jonathan Levine</td>
      <td>Joseph Gordon-Levitt</td>
      <td>Seth Rogen</td>
      <td>Anna Kendrick</td>
      <td>Bryce Dallas Howard</td>
      <td>315426</td>
      <td>35014192</td>
    </tr>
    <tr>
      <th>908</th>
      <td>Kick-Ass</td>
      <td>2010</td>
      <td>UA</td>
      <td>117</td>
      <td>Action, Comedy, Crime</td>
      <td>7.6</td>
      <td>Dave Lizewski is an unnoticed high school stud...</td>
      <td>66.00000</td>
      <td>Matthew Vaughn</td>
      <td>Aaron Taylor-Johnson</td>
      <td>Nicolas Cage</td>
      <td>Chloë Grace Moretz</td>
      <td>Garrett M. Brown</td>
      <td>524081</td>
      <td>48071303</td>
    </tr>
    <tr>
      <th>909</th>
      <td>Celda 211</td>
      <td>2009</td>
      <td>Unknown</td>
      <td>113</td>
      <td>Action, Adventure, Crime</td>
      <td>7.6</td>
      <td>The story of two men on different sides of a p...</td>
      <td>77.97153</td>
      <td>Daniel Monzón</td>
      <td>Luis Tosar</td>
      <td>Alberto Ammann</td>
      <td>Antonio Resines</td>
      <td>Manuel Morón</td>
      <td>63882</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>910</th>
      <td>Moneyball</td>
      <td>2011</td>
      <td>PG-13</td>
      <td>133</td>
      <td>Biography, Drama, Sport</td>
      <td>7.6</td>
      <td>Oakland A's general manager Billy Beane's succ...</td>
      <td>87.00000</td>
      <td>Bennett Miller</td>
      <td>Brad Pitt</td>
      <td>Robin Wright</td>
      <td>Jonah Hill</td>
      <td>Philip Seymour Hoffman</td>
      <td>369529</td>
      <td>75605492</td>
    </tr>
    <tr>
      <th>911</th>
      <td>La piel que habito</td>
      <td>2011</td>
      <td>R</td>
      <td>120</td>
      <td>Drama, Horror, Thriller</td>
      <td>7.6</td>
      <td>A brilliant plastic surgeon, haunted by past t...</td>
      <td>70.00000</td>
      <td>Pedro Almodóvar</td>
      <td>Antonio Banderas</td>
      <td>Elena Anaya</td>
      <td>Jan Cornet</td>
      <td>Marisa Paredes</td>
      <td>138959</td>
      <td>3185812</td>
    </tr>
    <tr>
      <th>912</th>
      <td>Zombieland</td>
      <td>2009</td>
      <td>A</td>
      <td>88</td>
      <td>Adventure, Comedy, Fantasy</td>
      <td>7.6</td>
      <td>A shy student trying to reach his family in Oh...</td>
      <td>73.00000</td>
      <td>Ruben Fleischer</td>
      <td>Jesse Eisenberg</td>
      <td>Emma Stone</td>
      <td>Woody Harrelson</td>
      <td>Abigail Breslin</td>
      <td>520041</td>
      <td>75590286</td>
    </tr>
    <tr>
      <th>913</th>
      <td>Die Welle</td>
      <td>2008</td>
      <td>Unknown</td>
      <td>107</td>
      <td>Drama, Thriller</td>
      <td>7.6</td>
      <td>A high school teacher's experiment to demonstr...</td>
      <td>77.97153</td>
      <td>Dennis Gansel</td>
      <td>Jürgen Vogel</td>
      <td>Frederick Lau</td>
      <td>Max Riemelt</td>
      <td>Jennifer Ulrich</td>
      <td>102742</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>914</th>
      <td>Sherlock Holmes</td>
      <td>2009</td>
      <td>PG-13</td>
      <td>128</td>
      <td>Action, Adventure, Mystery</td>
      <td>7.6</td>
      <td>Detective Sherlock Holmes and his stalwart par...</td>
      <td>57.00000</td>
      <td>Guy Ritchie</td>
      <td>Robert Downey Jr.</td>
      <td>Jude Law</td>
      <td>Rachel McAdams</td>
      <td>Mark Strong</td>
      <td>583158</td>
      <td>209028679</td>
    </tr>
    <tr>
      <th>915</th>
      <td>The Blind Side</td>
      <td>2009</td>
      <td>UA</td>
      <td>129</td>
      <td>Biography, Drama, Sport</td>
      <td>7.6</td>
      <td>The story of Michael Oher, a homeless and trau...</td>
      <td>53.00000</td>
      <td>John Lee Hancock</td>
      <td>Quinton Aaron</td>
      <td>Sandra Bullock</td>
      <td>Tim McGraw</td>
      <td>Jae Head</td>
      <td>293266</td>
      <td>255959475</td>
    </tr>
    <tr>
      <th>916</th>
      <td>The Visitor</td>
      <td>2007</td>
      <td>PG-13</td>
      <td>104</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>A college professor travels to New York City t...</td>
      <td>79.00000</td>
      <td>Tom McCarthy</td>
      <td>Richard Jenkins</td>
      <td>Haaz Sleiman</td>
      <td>Danai Gurira</td>
      <td>Hiam Abbass</td>
      <td>41544</td>
      <td>9422422</td>
    </tr>
    <tr>
      <th>917</th>
      <td>Seven Pounds</td>
      <td>2008</td>
      <td>UA</td>
      <td>123</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>A man with a fateful secret embarks on an extr...</td>
      <td>36.00000</td>
      <td>Gabriele Muccino</td>
      <td>Will Smith</td>
      <td>Rosario Dawson</td>
      <td>Woody Harrelson</td>
      <td>Michael Ealy</td>
      <td>286770</td>
      <td>69951824</td>
    </tr>
    <tr>
      <th>918</th>
      <td>Eastern Promises</td>
      <td>2007</td>
      <td>R</td>
      <td>100</td>
      <td>Action, Crime, Drama</td>
      <td>7.6</td>
      <td>A teenager who dies during childbirth leaves c...</td>
      <td>82.00000</td>
      <td>David Cronenberg</td>
      <td>Naomi Watts</td>
      <td>Viggo Mortensen</td>
      <td>Armin Mueller-Stahl</td>
      <td>Josef Altin</td>
      <td>227760</td>
      <td>17114882</td>
    </tr>
    <tr>
      <th>919</th>
      <td>Stardust</td>
      <td>2007</td>
      <td>U</td>
      <td>127</td>
      <td>Adventure, Family, Fantasy</td>
      <td>7.6</td>
      <td>In a countryside town bordering on a magical l...</td>
      <td>66.00000</td>
      <td>Matthew Vaughn</td>
      <td>Charlie Cox</td>
      <td>Claire Danes</td>
      <td>Sienna Miller</td>
      <td>Ian McKellen</td>
      <td>255036</td>
      <td>38634938</td>
    </tr>
    <tr>
      <th>920</th>
      <td>The Secret of Kells</td>
      <td>2009</td>
      <td>Unknown</td>
      <td>71</td>
      <td>Animation, Adventure, Family</td>
      <td>7.6</td>
      <td>A young boy in a remote medieval outpost under...</td>
      <td>81.00000</td>
      <td>Tomm Moore</td>
      <td>Nora Twomey</td>
      <td>Evan McGuire</td>
      <td>Brendan Gleeson</td>
      <td>Mick Lally</td>
      <td>31779</td>
      <td>686383</td>
    </tr>
    <tr>
      <th>921</th>
      <td>Inside Man</td>
      <td>2006</td>
      <td>R</td>
      <td>129</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.6</td>
      <td>A police detective, a bank robber, and a high-...</td>
      <td>76.00000</td>
      <td>Spike Lee</td>
      <td>Denzel Washington</td>
      <td>Clive Owen</td>
      <td>Jodie Foster</td>
      <td>Christopher Plummer</td>
      <td>339757</td>
      <td>88513495</td>
    </tr>
    <tr>
      <th>922</th>
      <td>Gone Baby Gone</td>
      <td>2007</td>
      <td>R</td>
      <td>114</td>
      <td>Crime, Drama, Mystery</td>
      <td>7.6</td>
      <td>Two Boston area detectives investigate a littl...</td>
      <td>72.00000</td>
      <td>Ben Affleck</td>
      <td>Morgan Freeman</td>
      <td>Ed Harris</td>
      <td>Casey Affleck</td>
      <td>Michelle Monaghan</td>
      <td>250590</td>
      <td>20300218</td>
    </tr>
    <tr>
      <th>923</th>
      <td>La Vie En Rose</td>
      <td>2007</td>
      <td>PG-13</td>
      <td>140</td>
      <td>Biography, Drama, Music</td>
      <td>7.6</td>
      <td>Biopic of the iconic French singer Édith Piaf....</td>
      <td>66.00000</td>
      <td>Olivier Dahan</td>
      <td>Marion Cotillard</td>
      <td>Sylvie Testud</td>
      <td>Pascal Greggory</td>
      <td>Emmanuelle Seigner</td>
      <td>82781</td>
      <td>10301706</td>
    </tr>
    <tr>
      <th>924</th>
      <td>Huo Yuan Jia</td>
      <td>2006</td>
      <td>PG-13</td>
      <td>104</td>
      <td>Action, Biography, Drama</td>
      <td>7.6</td>
      <td>A biography of Chinese Martial Arts Master Huo...</td>
      <td>70.00000</td>
      <td>Ronny Yu</td>
      <td>Jet Li</td>
      <td>Li Sun</td>
      <td>Yong Dong</td>
      <td>Yun Qu</td>
      <td>72863</td>
      <td>24633730</td>
    </tr>
    <tr>
      <th>925</th>
      <td>The Illusionist</td>
      <td>2006</td>
      <td>U</td>
      <td>110</td>
      <td>Drama, Fantasy, Mystery</td>
      <td>7.6</td>
      <td>In turn-of-the-century Vienna, a magician uses...</td>
      <td>68.00000</td>
      <td>Neil Burger</td>
      <td>Edward Norton</td>
      <td>Jessica Biel</td>
      <td>Paul Giamatti</td>
      <td>Rufus Sewell</td>
      <td>354728</td>
      <td>39868642</td>
    </tr>
    <tr>
      <th>926</th>
      <td>Dead Man's Shoes</td>
      <td>2004</td>
      <td>Unknown</td>
      <td>90</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.6</td>
      <td>A disaffected soldier returns to his hometown ...</td>
      <td>52.00000</td>
      <td>Shane Meadows</td>
      <td>Paddy Considine</td>
      <td>Gary Stretch</td>
      <td>Toby Kebbell</td>
      <td>Stuart Wolfenden</td>
      <td>49728</td>
      <td>6013</td>
    </tr>
    <tr>
      <th>927</th>
      <td>Harry Potter and the Half-Blood Prince</td>
      <td>2009</td>
      <td>UA</td>
      <td>153</td>
      <td>Action, Adventure, Family</td>
      <td>7.6</td>
      <td>As Harry Potter begins his sixth year at Hogwa...</td>
      <td>78.00000</td>
      <td>David Yates</td>
      <td>Daniel Radcliffe</td>
      <td>Emma Watson</td>
      <td>Rupert Grint</td>
      <td>Michael Gambon</td>
      <td>474827</td>
      <td>301959197</td>
    </tr>
    <tr>
      <th>928</th>
      <td>300</td>
      <td>2006</td>
      <td>A</td>
      <td>117</td>
      <td>Action, Drama</td>
      <td>7.6</td>
      <td>King Leonidas of Sparta and a force of 300 men...</td>
      <td>52.00000</td>
      <td>Zack Snyder</td>
      <td>Gerard Butler</td>
      <td>Lena Headey</td>
      <td>David Wenham</td>
      <td>Dominic West</td>
      <td>732876</td>
      <td>210614939</td>
    </tr>
    <tr>
      <th>929</th>
      <td>Match Point</td>
      <td>2005</td>
      <td>R</td>
      <td>124</td>
      <td>Drama, Romance, Thriller</td>
      <td>7.6</td>
      <td>At a turning point in his life, a former tenni...</td>
      <td>72.00000</td>
      <td>Woody Allen</td>
      <td>Scarlett Johansson</td>
      <td>Jonathan Rhys Meyers</td>
      <td>Emily Mortimer</td>
      <td>Matthew Goode</td>
      <td>206294</td>
      <td>23089926</td>
    </tr>
    <tr>
      <th>930</th>
      <td>Watchmen</td>
      <td>2009</td>
      <td>A</td>
      <td>162</td>
      <td>Action, Drama, Mystery</td>
      <td>7.6</td>
      <td>In 1985 where former superheroes exist, the mu...</td>
      <td>56.00000</td>
      <td>Zack Snyder</td>
      <td>Jackie Earle Haley</td>
      <td>Patrick Wilson</td>
      <td>Carla Gugino</td>
      <td>Malin Akerman</td>
      <td>500799</td>
      <td>107509799</td>
    </tr>
    <tr>
      <th>931</th>
      <td>Lord of War</td>
      <td>2005</td>
      <td>R</td>
      <td>122</td>
      <td>Action, Crime, Drama</td>
      <td>7.6</td>
      <td>An arms dealer confronts the morality of his w...</td>
      <td>62.00000</td>
      <td>Andrew Niccol</td>
      <td>Nicolas Cage</td>
      <td>Ethan Hawke</td>
      <td>Jared Leto</td>
      <td>Bridget Moynahan</td>
      <td>294140</td>
      <td>24149632</td>
    </tr>
    <tr>
      <th>932</th>
      <td>Saw</td>
      <td>2004</td>
      <td>UA</td>
      <td>103</td>
      <td>Horror, Mystery, Thriller</td>
      <td>7.6</td>
      <td>Two strangers awaken in a room with no recolle...</td>
      <td>46.00000</td>
      <td>James Wan</td>
      <td>Cary Elwes</td>
      <td>Leigh Whannell</td>
      <td>Danny Glover</td>
      <td>Ken Leung</td>
      <td>379020</td>
      <td>56000369</td>
    </tr>
    <tr>
      <th>933</th>
      <td>Synecdoche, New York</td>
      <td>2008</td>
      <td>R</td>
      <td>124</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>A theatre director struggles with his work, an...</td>
      <td>67.00000</td>
      <td>Charlie Kaufman</td>
      <td>Philip Seymour Hoffman</td>
      <td>Samantha Morton</td>
      <td>Michelle Williams</td>
      <td>Catherine Keener</td>
      <td>83158</td>
      <td>3081925</td>
    </tr>
    <tr>
      <th>934</th>
      <td>Mysterious Skin</td>
      <td>2004</td>
      <td>R</td>
      <td>105</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>A teenage hustler and a young man obsessed wit...</td>
      <td>73.00000</td>
      <td>Gregg Araki</td>
      <td>Brady Corbet</td>
      <td>Joseph Gordon-Levitt</td>
      <td>Elisabeth Shue</td>
      <td>Chase Ellison</td>
      <td>65939</td>
      <td>697181</td>
    </tr>
    <tr>
      <th>935</th>
      <td>Jeux d'enfants</td>
      <td>2003</td>
      <td>R</td>
      <td>93</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.6</td>
      <td>As adults, best friends Julien and Sophie cont...</td>
      <td>45.00000</td>
      <td>Yann Samuell</td>
      <td>Guillaume Canet</td>
      <td>Marion Cotillard</td>
      <td>Thibault Verhaeghe</td>
      <td>Joséphine Lebas-Joly</td>
      <td>67360</td>
      <td>548707</td>
    </tr>
    <tr>
      <th>936</th>
      <td>Un long dimanche de fiançailles</td>
      <td>2004</td>
      <td>U</td>
      <td>133</td>
      <td>Drama, Mystery, Romance</td>
      <td>7.6</td>
      <td>Tells the story of a young woman's relentless ...</td>
      <td>76.00000</td>
      <td>Jean-Pierre Jeunet</td>
      <td>Audrey Tautou</td>
      <td>Gaspard Ulliel</td>
      <td>Jodie Foster</td>
      <td>Dominique Pinon</td>
      <td>70925</td>
      <td>6167817</td>
    </tr>
    <tr>
      <th>937</th>
      <td>The Station Agent</td>
      <td>2003</td>
      <td>R</td>
      <td>89</td>
      <td>Comedy, Drama</td>
      <td>7.6</td>
      <td>When his only friend dies, a man born with dwa...</td>
      <td>81.00000</td>
      <td>Tom McCarthy</td>
      <td>Peter Dinklage</td>
      <td>Patricia Clarkson</td>
      <td>Bobby Cannavale</td>
      <td>Paul Benjamin</td>
      <td>67370</td>
      <td>5739376</td>
    </tr>
    <tr>
      <th>938</th>
      <td>21 Grams</td>
      <td>2003</td>
      <td>UA</td>
      <td>124</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.6</td>
      <td>A freak accident brings together a critically ...</td>
      <td>70.00000</td>
      <td>Alejandro G. Iñárritu</td>
      <td>Sean Penn</td>
      <td>Benicio Del Toro</td>
      <td>Naomi Watts</td>
      <td>Danny Huston</td>
      <td>224545</td>
      <td>16290476</td>
    </tr>
    <tr>
      <th>939</th>
      <td>Boksuneun naui geot</td>
      <td>2002</td>
      <td>R</td>
      <td>129</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.6</td>
      <td>A recently laid off factory worker kidnaps his...</td>
      <td>56.00000</td>
      <td>Chan-wook Park</td>
      <td>Kang-ho Song</td>
      <td>Shin Ha-kyun</td>
      <td>Bae Doona</td>
      <td>Ji-Eun Lim</td>
      <td>62659</td>
      <td>45289</td>
    </tr>
    <tr>
      <th>940</th>
      <td>Finding Neverland</td>
      <td>2004</td>
      <td>U</td>
      <td>106</td>
      <td>Biography, Drama, Family</td>
      <td>7.6</td>
      <td>The story of Sir J.M. Barrie's friendship with...</td>
      <td>67.00000</td>
      <td>Marc Forster</td>
      <td>Johnny Depp</td>
      <td>Kate Winslet</td>
      <td>Julie Christie</td>
      <td>Radha Mitchell</td>
      <td>198677</td>
      <td>51680613</td>
    </tr>
    <tr>
      <th>941</th>
      <td>25th Hour</td>
      <td>2002</td>
      <td>R</td>
      <td>135</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>Cornered by the DEA, convicted New York drug d...</td>
      <td>68.00000</td>
      <td>Spike Lee</td>
      <td>Edward Norton</td>
      <td>Barry Pepper</td>
      <td>Philip Seymour Hoffman</td>
      <td>Rosario Dawson</td>
      <td>169708</td>
      <td>13060843</td>
    </tr>
    <tr>
      <th>942</th>
      <td>The Butterfly Effect</td>
      <td>2004</td>
      <td>U</td>
      <td>113</td>
      <td>Drama, Sci-Fi, Thriller</td>
      <td>7.6</td>
      <td>Evan Treborn suffers blackouts during signific...</td>
      <td>30.00000</td>
      <td>Eric Bress</td>
      <td>J. Mackye Gruber</td>
      <td>Ashton Kutcher</td>
      <td>Amy Smart</td>
      <td>Melora Walters</td>
      <td>451479</td>
      <td>57938693</td>
    </tr>
    <tr>
      <th>943</th>
      <td>28 Days Later...</td>
      <td>2002</td>
      <td>A</td>
      <td>113</td>
      <td>Drama, Horror, Sci-Fi</td>
      <td>7.6</td>
      <td>Four weeks after a mysterious, incurable virus...</td>
      <td>73.00000</td>
      <td>Danny Boyle</td>
      <td>Cillian Murphy</td>
      <td>Naomie Harris</td>
      <td>Christopher Eccleston</td>
      <td>Alex Palmer</td>
      <td>376853</td>
      <td>45064915</td>
    </tr>
    <tr>
      <th>944</th>
      <td>Batoru rowaiaru</td>
      <td>2000</td>
      <td>Unknown</td>
      <td>114</td>
      <td>Action, Adventure, Drama</td>
      <td>7.6</td>
      <td>In the future, the Japanese government capture...</td>
      <td>81.00000</td>
      <td>Kinji Fukasaku</td>
      <td>Tatsuya Fujiwara</td>
      <td>Aki Maeda</td>
      <td>Tarô Yamamoto</td>
      <td>Takeshi Kitano</td>
      <td>169091</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>945</th>
      <td>The Royal Tenenbaums</td>
      <td>2001</td>
      <td>A</td>
      <td>110</td>
      <td>Comedy, Drama</td>
      <td>7.6</td>
      <td>The eccentric members of a dysfunctional famil...</td>
      <td>76.00000</td>
      <td>Wes Anderson</td>
      <td>Gene Hackman</td>
      <td>Gwyneth Paltrow</td>
      <td>Anjelica Huston</td>
      <td>Ben Stiller</td>
      <td>266842</td>
      <td>52364010</td>
    </tr>
    <tr>
      <th>946</th>
      <td>Y tu mamá también</td>
      <td>2001</td>
      <td>A</td>
      <td>106</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>In Mexico, two teenage boys and an attractive ...</td>
      <td>88.00000</td>
      <td>Alfonso Cuarón</td>
      <td>Maribel Verdú</td>
      <td>Gael García Bernal</td>
      <td>Daniel Giménez Cacho</td>
      <td>Ana López Mercado</td>
      <td>115827</td>
      <td>13622333</td>
    </tr>
    <tr>
      <th>947</th>
      <td>Harry Potter and the Sorcerer's Stone</td>
      <td>2001</td>
      <td>U</td>
      <td>152</td>
      <td>Adventure, Family, Fantasy</td>
      <td>7.6</td>
      <td>An orphaned boy enrolls in a school of wizardr...</td>
      <td>64.00000</td>
      <td>Chris Columbus</td>
      <td>Daniel Radcliffe</td>
      <td>Rupert Grint</td>
      <td>Richard Harris</td>
      <td>Maggie Smith</td>
      <td>658185</td>
      <td>317575550</td>
    </tr>
    <tr>
      <th>948</th>
      <td>The Others</td>
      <td>2001</td>
      <td>PG-13</td>
      <td>101</td>
      <td>Horror, Mystery, Thriller</td>
      <td>7.6</td>
      <td>A woman who lives in her darkened old family h...</td>
      <td>74.00000</td>
      <td>Alejandro Amenábar</td>
      <td>Nicole Kidman</td>
      <td>Christopher Eccleston</td>
      <td>Fionnula Flanagan</td>
      <td>Alakina Mann</td>
      <td>337651</td>
      <td>96522687</td>
    </tr>
    <tr>
      <th>949</th>
      <td>Blow</td>
      <td>2001</td>
      <td>R</td>
      <td>124</td>
      <td>Biography, Crime, Drama</td>
      <td>7.6</td>
      <td>The story of how George Jung, along with the M...</td>
      <td>52.00000</td>
      <td>Ted Demme</td>
      <td>Johnny Depp</td>
      <td>Penélope Cruz</td>
      <td>Franka Potente</td>
      <td>Rachel Griffiths</td>
      <td>240714</td>
      <td>52990775</td>
    </tr>
    <tr>
      <th>950</th>
      <td>Enemy at the Gates</td>
      <td>2001</td>
      <td>A</td>
      <td>131</td>
      <td>Drama, History, War</td>
      <td>7.6</td>
      <td>A Russian and a German sniper play a game of c...</td>
      <td>53.00000</td>
      <td>Jean-Jacques Annaud</td>
      <td>Jude Law</td>
      <td>Ed Harris</td>
      <td>Joseph Fiennes</td>
      <td>Rachel Weisz</td>
      <td>243729</td>
      <td>51401758</td>
    </tr>
    <tr>
      <th>951</th>
      <td>Minority Report</td>
      <td>2002</td>
      <td>A</td>
      <td>145</td>
      <td>Action, Crime, Mystery</td>
      <td>7.6</td>
      <td>In a future where a special police unit is abl...</td>
      <td>80.00000</td>
      <td>Steven Spielberg</td>
      <td>Tom Cruise</td>
      <td>Colin Farrell</td>
      <td>Samantha Morton</td>
      <td>Max von Sydow</td>
      <td>508417</td>
      <td>132072926</td>
    </tr>
    <tr>
      <th>952</th>
      <td>The Hurricane</td>
      <td>1999</td>
      <td>R</td>
      <td>146</td>
      <td>Biography, Drama, Sport</td>
      <td>7.6</td>
      <td>The story of Rubin 'Hurricane' Carter, a boxer...</td>
      <td>74.00000</td>
      <td>Norman Jewison</td>
      <td>Denzel Washington</td>
      <td>Vicellous Shannon</td>
      <td>Deborah Kara Unger</td>
      <td>Liev Schreiber</td>
      <td>91557</td>
      <td>50668906</td>
    </tr>
    <tr>
      <th>953</th>
      <td>American Psycho</td>
      <td>2000</td>
      <td>A</td>
      <td>101</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.6</td>
      <td>A wealthy New York City investment banking exe...</td>
      <td>64.00000</td>
      <td>Mary Harron</td>
      <td>Christian Bale</td>
      <td>Justin Theroux</td>
      <td>Josh Lucas</td>
      <td>Bill Sage</td>
      <td>490062</td>
      <td>15070285</td>
    </tr>
    <tr>
      <th>954</th>
      <td>Lola rennt</td>
      <td>1998</td>
      <td>UA</td>
      <td>81</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.6</td>
      <td>After a botched money delivery, Lola has 20 mi...</td>
      <td>77.00000</td>
      <td>Tom Tykwer</td>
      <td>Franka Potente</td>
      <td>Moritz Bleibtreu</td>
      <td>Herbert Knaup</td>
      <td>Nina Petri</td>
      <td>188317</td>
      <td>7267585</td>
    </tr>
    <tr>
      <th>955</th>
      <td>The Thin Red Line</td>
      <td>1998</td>
      <td>A</td>
      <td>170</td>
      <td>Drama, War</td>
      <td>7.6</td>
      <td>Adaptation of James Jones' autobiographical 19...</td>
      <td>78.00000</td>
      <td>Terrence Malick</td>
      <td>Jim Caviezel</td>
      <td>Sean Penn</td>
      <td>Nick Nolte</td>
      <td>Kirk Acevedo</td>
      <td>172710</td>
      <td>36400491</td>
    </tr>
    <tr>
      <th>956</th>
      <td>Mulan</td>
      <td>1998</td>
      <td>U</td>
      <td>88</td>
      <td>Animation, Adventure, Family</td>
      <td>7.6</td>
      <td>To save her father from death in the army, a y...</td>
      <td>71.00000</td>
      <td>Tony Bancroft</td>
      <td>Barry Cook</td>
      <td>Ming-Na Wen</td>
      <td>Eddie Murphy</td>
      <td>BD Wong</td>
      <td>256906</td>
      <td>120620254</td>
    </tr>
    <tr>
      <th>957</th>
      <td>Fear and Loathing in Las Vegas</td>
      <td>1998</td>
      <td>R</td>
      <td>118</td>
      <td>Adventure, Comedy, Drama</td>
      <td>7.6</td>
      <td>An oddball journalist and his psychopathic law...</td>
      <td>41.00000</td>
      <td>Terry Gilliam</td>
      <td>Johnny Depp</td>
      <td>Benicio Del Toro</td>
      <td>Tobey Maguire</td>
      <td>Michael Lee Gogin</td>
      <td>259753</td>
      <td>10680275</td>
    </tr>
    <tr>
      <th>958</th>
      <td>Funny Games</td>
      <td>1997</td>
      <td>A</td>
      <td>108</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.6</td>
      <td>Two violent young men take a mother, father, a...</td>
      <td>69.00000</td>
      <td>Michael Haneke</td>
      <td>Susanne Lothar</td>
      <td>Ulrich Mühe</td>
      <td>Arno Frisch</td>
      <td>Frank Giering</td>
      <td>65058</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>959</th>
      <td>Dark City</td>
      <td>1998</td>
      <td>A</td>
      <td>100</td>
      <td>Mystery, Sci-Fi, Thriller</td>
      <td>7.6</td>
      <td>A man struggles with memories of his past, whi...</td>
      <td>66.00000</td>
      <td>Alex Proyas</td>
      <td>Rufus Sewell</td>
      <td>Kiefer Sutherland</td>
      <td>Jennifer Connelly</td>
      <td>William Hurt</td>
      <td>187927</td>
      <td>14378331</td>
    </tr>
    <tr>
      <th>960</th>
      <td>Sleepers</td>
      <td>1996</td>
      <td>UA</td>
      <td>147</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.6</td>
      <td>After a prank goes disastrously wrong, a group...</td>
      <td>49.00000</td>
      <td>Barry Levinson</td>
      <td>Robert De Niro</td>
      <td>Kevin Bacon</td>
      <td>Brad Pitt</td>
      <td>Jason Patric</td>
      <td>186734</td>
      <td>49100000</td>
    </tr>
    <tr>
      <th>961</th>
      <td>Lost Highway</td>
      <td>1997</td>
      <td>A</td>
      <td>134</td>
      <td>Mystery, Thriller</td>
      <td>7.6</td>
      <td>Anonymous videotapes presage a musician's murd...</td>
      <td>52.00000</td>
      <td>David Lynch</td>
      <td>Bill Pullman</td>
      <td>Patricia Arquette</td>
      <td>John Roselius</td>
      <td>Louis Eppolito</td>
      <td>131101</td>
      <td>3796699</td>
    </tr>
    <tr>
      <th>962</th>
      <td>Sense and Sensibility</td>
      <td>1995</td>
      <td>U</td>
      <td>136</td>
      <td>Drama, Romance</td>
      <td>7.6</td>
      <td>Rich Mr. Dashwood dies, leaving his second wif...</td>
      <td>84.00000</td>
      <td>Ang Lee</td>
      <td>Emma Thompson</td>
      <td>Kate Winslet</td>
      <td>James Fleet</td>
      <td>Tom Wilkinson</td>
      <td>102598</td>
      <td>43182776</td>
    </tr>
    <tr>
      <th>963</th>
      <td>Die Hard: With a Vengeance</td>
      <td>1995</td>
      <td>A</td>
      <td>128</td>
      <td>Action, Adventure, Thriller</td>
      <td>7.6</td>
      <td>John McClane and a Harlem store owner are targ...</td>
      <td>58.00000</td>
      <td>John McTiernan</td>
      <td>Bruce Willis</td>
      <td>Jeremy Irons</td>
      <td>Samuel L. Jackson</td>
      <td>Graham Greene</td>
      <td>364420</td>
      <td>100012499</td>
    </tr>
    <tr>
      <th>964</th>
      <td>Dead Man</td>
      <td>1995</td>
      <td>R</td>
      <td>121</td>
      <td>Adventure, Drama, Fantasy</td>
      <td>7.6</td>
      <td>On the run after murdering a man, accountant W...</td>
      <td>62.00000</td>
      <td>Jim Jarmusch</td>
      <td>Johnny Depp</td>
      <td>Gary Farmer</td>
      <td>Crispin Glover</td>
      <td>Lance Henriksen</td>
      <td>90442</td>
      <td>1037847</td>
    </tr>
    <tr>
      <th>965</th>
      <td>The Bridges of Madison County</td>
      <td>1995</td>
      <td>A</td>
      <td>135</td>
      <td>Drama, Romance</td>
      <td>7.6</td>
      <td>Photographer Robert Kincaid wanders into the l...</td>
      <td>69.00000</td>
      <td>Clint Eastwood</td>
      <td>Clint Eastwood</td>
      <td>Meryl Streep</td>
      <td>Annie Corley</td>
      <td>Victor Slezak</td>
      <td>73172</td>
      <td>71516617</td>
    </tr>
    <tr>
      <th>967</th>
      <td>Trois couleurs: Blanc</td>
      <td>1994</td>
      <td>U</td>
      <td>92</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.6</td>
      <td>After his wife divorces him, a Polish immigran...</td>
      <td>88.00000</td>
      <td>Krzysztof Kieslowski</td>
      <td>Zbigniew Zamachowski</td>
      <td>Julie Delpy</td>
      <td>Janusz Gajos</td>
      <td>Jerzy Stuhr</td>
      <td>64390</td>
      <td>1464625</td>
    </tr>
    <tr>
      <th>968</th>
      <td>Falling Down</td>
      <td>1993</td>
      <td>R</td>
      <td>113</td>
      <td>Action, Crime, Drama</td>
      <td>7.6</td>
      <td>An ordinary man frustrated with the various fl...</td>
      <td>56.00000</td>
      <td>Joel Schumacher</td>
      <td>Michael Douglas</td>
      <td>Robert Duvall</td>
      <td>Barbara Hershey</td>
      <td>Rachel Ticotin</td>
      <td>171640</td>
      <td>40903593</td>
    </tr>
    <tr>
      <th>969</th>
      <td>Dazed and Confused</td>
      <td>1993</td>
      <td>U</td>
      <td>102</td>
      <td>Comedy</td>
      <td>7.6</td>
      <td>The adventures of high school and junior high ...</td>
      <td>78.00000</td>
      <td>Richard Linklater</td>
      <td>Jason London</td>
      <td>Wiley Wiggins</td>
      <td>Matthew McConaughey</td>
      <td>Rory Cochrane</td>
      <td>165465</td>
      <td>7993039</td>
    </tr>
    <tr>
      <th>970</th>
      <td>My Cousin Vinny</td>
      <td>1992</td>
      <td>UA</td>
      <td>120</td>
      <td>Comedy, Crime</td>
      <td>7.6</td>
      <td>Two New Yorkers accused of murder in rural Ala...</td>
      <td>68.00000</td>
      <td>Jonathan Lynn</td>
      <td>Joe Pesci</td>
      <td>Marisa Tomei</td>
      <td>Ralph Macchio</td>
      <td>Mitchell Whitfield</td>
      <td>107325</td>
      <td>52929168</td>
    </tr>
    <tr>
      <th>971</th>
      <td>Omohide poro poro</td>
      <td>1991</td>
      <td>U</td>
      <td>118</td>
      <td>Animation, Drama, Romance</td>
      <td>7.6</td>
      <td>A twenty-seven-year-old office worker travels ...</td>
      <td>90.00000</td>
      <td>Isao Takahata</td>
      <td>Miki Imai</td>
      <td>Toshirô Yanagiba</td>
      <td>Yoko Honna</td>
      <td>Mayumi Izuka</td>
      <td>27071</td>
      <td>453243</td>
    </tr>
    <tr>
      <th>972</th>
      <td>Delicatessen</td>
      <td>1991</td>
      <td>R</td>
      <td>99</td>
      <td>Comedy, Crime</td>
      <td>7.6</td>
      <td>Post-apocalyptic surrealist black comedy about...</td>
      <td>66.00000</td>
      <td>Marc Caro</td>
      <td>Jean-Pierre Jeunet</td>
      <td>Marie-Laure Dougnac</td>
      <td>Dominique Pinon</td>
      <td>Pascal Benezech</td>
      <td>80487</td>
      <td>1794187</td>
    </tr>
    <tr>
      <th>973</th>
      <td>Home Alone</td>
      <td>1990</td>
      <td>U</td>
      <td>103</td>
      <td>Comedy, Family</td>
      <td>7.6</td>
      <td>An eight-year-old troublemaker must protect hi...</td>
      <td>63.00000</td>
      <td>Chris Columbus</td>
      <td>Macaulay Culkin</td>
      <td>Joe Pesci</td>
      <td>Daniel Stern</td>
      <td>John Heard</td>
      <td>488817</td>
      <td>285761243</td>
    </tr>
    <tr>
      <th>974</th>
      <td>The Godfather: Part III</td>
      <td>1990</td>
      <td>A</td>
      <td>162</td>
      <td>Crime, Drama</td>
      <td>7.6</td>
      <td>Follows Michael Corleone, now in his 60s, as h...</td>
      <td>60.00000</td>
      <td>Francis Ford Coppola</td>
      <td>Al Pacino</td>
      <td>Diane Keaton</td>
      <td>Andy Garcia</td>
      <td>Talia Shire</td>
      <td>359809</td>
      <td>66666062</td>
    </tr>
    <tr>
      <th>975</th>
      <td>When Harry Met Sally...</td>
      <td>1989</td>
      <td>UA</td>
      <td>95</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.6</td>
      <td>Harry and Sally have known each other for year...</td>
      <td>76.00000</td>
      <td>Rob Reiner</td>
      <td>Billy Crystal</td>
      <td>Meg Ryan</td>
      <td>Carrie Fisher</td>
      <td>Bruno Kirby</td>
      <td>195663</td>
      <td>92823600</td>
    </tr>
    <tr>
      <th>976</th>
      <td>The Little Mermaid</td>
      <td>1989</td>
      <td>U</td>
      <td>83</td>
      <td>Animation, Family, Fantasy</td>
      <td>7.6</td>
      <td>A mermaid princess makes a Faustian bargain in...</td>
      <td>88.00000</td>
      <td>Ron Clements</td>
      <td>John Musker</td>
      <td>Jodi Benson</td>
      <td>Samuel E. Wright</td>
      <td>Rene Auberjonois</td>
      <td>237696</td>
      <td>111543479</td>
    </tr>
    <tr>
      <th>977</th>
      <td>The Naked Gun: From the Files of Police Squad!</td>
      <td>1988</td>
      <td>U</td>
      <td>85</td>
      <td>Comedy, Crime</td>
      <td>7.6</td>
      <td>Incompetent police Detective Frank Drebin must...</td>
      <td>76.00000</td>
      <td>David Zucker</td>
      <td>Leslie Nielsen</td>
      <td>Priscilla Presley</td>
      <td>O.J. Simpson</td>
      <td>Ricardo Montalban</td>
      <td>152871</td>
      <td>78756177</td>
    </tr>
    <tr>
      <th>978</th>
      <td>Planes, Trains &amp; Automobiles</td>
      <td>1987</td>
      <td>U</td>
      <td>93</td>
      <td>Comedy, Drama</td>
      <td>7.6</td>
      <td>A man must struggle to travel home for Thanksg...</td>
      <td>72.00000</td>
      <td>John Hughes</td>
      <td>Steve Martin</td>
      <td>John Candy</td>
      <td>Laila Robins</td>
      <td>Michael McKean</td>
      <td>124773</td>
      <td>49530280</td>
    </tr>
    <tr>
      <th>979</th>
      <td>Lethal Weapon</td>
      <td>1987</td>
      <td>A</td>
      <td>109</td>
      <td>Action, Crime, Thriller</td>
      <td>7.6</td>
      <td>Two newly paired cops who are complete opposit...</td>
      <td>68.00000</td>
      <td>Richard Donner</td>
      <td>Mel Gibson</td>
      <td>Danny Glover</td>
      <td>Gary Busey</td>
      <td>Mitchell Ryan</td>
      <td>236894</td>
      <td>65207127</td>
    </tr>
    <tr>
      <th>980</th>
      <td>Blood Simple</td>
      <td>1984</td>
      <td>A</td>
      <td>99</td>
      <td>Crime, Drama, Thriller</td>
      <td>7.6</td>
      <td>The owner of a seedy small-town Texas bar disc...</td>
      <td>82.00000</td>
      <td>Joel Coen</td>
      <td>Ethan Coen</td>
      <td>John Getz</td>
      <td>Frances McDormand</td>
      <td>Dan Hedaya</td>
      <td>87745</td>
      <td>2150000</td>
    </tr>
    <tr>
      <th>981</th>
      <td>On Golden Pond</td>
      <td>1981</td>
      <td>UA</td>
      <td>109</td>
      <td>Drama</td>
      <td>7.6</td>
      <td>Norman is a curmudgeon with an estranged relat...</td>
      <td>68.00000</td>
      <td>Mark Rydell</td>
      <td>Katharine Hepburn</td>
      <td>Henry Fonda</td>
      <td>Jane Fonda</td>
      <td>Doug McKeon</td>
      <td>27650</td>
      <td>119285432</td>
    </tr>
    <tr>
      <th>982</th>
      <td>Mad Max 2</td>
      <td>1981</td>
      <td>A</td>
      <td>96</td>
      <td>Action, Adventure, Sci-Fi</td>
      <td>7.6</td>
      <td>In the post-apocalyptic Australian wasteland, ...</td>
      <td>77.00000</td>
      <td>George Miller</td>
      <td>Mel Gibson</td>
      <td>Bruce Spence</td>
      <td>Michael Preston</td>
      <td>Max Phipps</td>
      <td>166588</td>
      <td>12465371</td>
    </tr>
    <tr>
      <th>983</th>
      <td>The Warriors</td>
      <td>1979</td>
      <td>UA</td>
      <td>92</td>
      <td>Action, Crime, Thriller</td>
      <td>7.6</td>
      <td>In the near future, a charismatic leader summo...</td>
      <td>65.00000</td>
      <td>Walter Hill</td>
      <td>Michael Beck</td>
      <td>James Remar</td>
      <td>Dorsey Wright</td>
      <td>Brian Tyler</td>
      <td>93878</td>
      <td>22490039</td>
    </tr>
    <tr>
      <th>984</th>
      <td>The Muppet Movie</td>
      <td>1979</td>
      <td>U</td>
      <td>95</td>
      <td>Adventure, Comedy, Family</td>
      <td>7.6</td>
      <td>Kermit and his newfound friends trek across Am...</td>
      <td>74.00000</td>
      <td>James Frawley</td>
      <td>Jim Henson</td>
      <td>Frank Oz</td>
      <td>Jerry Nelson</td>
      <td>Richard Hunt</td>
      <td>32802</td>
      <td>76657000</td>
    </tr>
    <tr>
      <th>985</th>
      <td>Escape from Alcatraz</td>
      <td>1979</td>
      <td>A</td>
      <td>112</td>
      <td>Action, Biography, Crime</td>
      <td>7.6</td>
      <td>Alcatraz is the most secure prison of its time...</td>
      <td>76.00000</td>
      <td>Don Siegel</td>
      <td>Clint Eastwood</td>
      <td>Patrick McGoohan</td>
      <td>Roberts Blossom</td>
      <td>Jack Thibeau</td>
      <td>121731</td>
      <td>43000000</td>
    </tr>
    <tr>
      <th>986</th>
      <td>Watership Down</td>
      <td>1978</td>
      <td>U</td>
      <td>91</td>
      <td>Animation, Adventure, Drama</td>
      <td>7.6</td>
      <td>Hoping to escape destruction by human develope...</td>
      <td>64.00000</td>
      <td>Martin Rosen</td>
      <td>John Hubley</td>
      <td>John Hurt</td>
      <td>Richard Briers</td>
      <td>Ralph Richardson</td>
      <td>33656</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>987</th>
      <td>Midnight Express</td>
      <td>1978</td>
      <td>A</td>
      <td>121</td>
      <td>Biography, Crime, Drama</td>
      <td>7.6</td>
      <td>Billy Hayes, an American college student, is c...</td>
      <td>59.00000</td>
      <td>Alan Parker</td>
      <td>Brad Davis</td>
      <td>Irene Miracle</td>
      <td>Bo Hopkins</td>
      <td>Paolo Bonacelli</td>
      <td>73662</td>
      <td>35000000</td>
    </tr>
    <tr>
      <th>988</th>
      <td>Close Encounters of the Third Kind</td>
      <td>1977</td>
      <td>U</td>
      <td>138</td>
      <td>Drama, Sci-Fi</td>
      <td>7.6</td>
      <td>Roy Neary, an electric lineman, watches how hi...</td>
      <td>90.00000</td>
      <td>Steven Spielberg</td>
      <td>Richard Dreyfuss</td>
      <td>François Truffaut</td>
      <td>Teri Garr</td>
      <td>Melinda Dillon</td>
      <td>184966</td>
      <td>132088635</td>
    </tr>
    <tr>
      <th>989</th>
      <td>The Long Goodbye</td>
      <td>1973</td>
      <td>A</td>
      <td>112</td>
      <td>Comedy, Crime, Drama</td>
      <td>7.6</td>
      <td>Private investigator Philip Marlowe helps a fr...</td>
      <td>87.00000</td>
      <td>Robert Altman</td>
      <td>Elliott Gould</td>
      <td>Nina van Pallandt</td>
      <td>Sterling Hayden</td>
      <td>Mark Rydell</td>
      <td>26337</td>
      <td>959000</td>
    </tr>
    <tr>
      <th>990</th>
      <td>Giù la testa</td>
      <td>1971</td>
      <td>PG</td>
      <td>157</td>
      <td>Drama, War, Western</td>
      <td>7.6</td>
      <td>A low-life bandit and an I.R.A. explosives exp...</td>
      <td>77.00000</td>
      <td>Sergio Leone</td>
      <td>Rod Steiger</td>
      <td>James Coburn</td>
      <td>Romolo Valli</td>
      <td>Maria Monti</td>
      <td>30144</td>
      <td>696690</td>
    </tr>
    <tr>
      <th>991</th>
      <td>Kelly's Heroes</td>
      <td>1970</td>
      <td>GP</td>
      <td>144</td>
      <td>Adventure, Comedy, War</td>
      <td>7.6</td>
      <td>A group of U.S. soldiers sneaks across enemy l...</td>
      <td>50.00000</td>
      <td>Brian G. Hutton</td>
      <td>Clint Eastwood</td>
      <td>Telly Savalas</td>
      <td>Don Rickles</td>
      <td>Carroll O'Connor</td>
      <td>45338</td>
      <td>1378435</td>
    </tr>
    <tr>
      <th>992</th>
      <td>The Jungle Book</td>
      <td>1967</td>
      <td>U</td>
      <td>78</td>
      <td>Animation, Adventure, Family</td>
      <td>7.6</td>
      <td>Bagheera the Panther and Baloo the Bear have a...</td>
      <td>65.00000</td>
      <td>Wolfgang Reitherman</td>
      <td>Phil Harris</td>
      <td>Sebastian Cabot</td>
      <td>Louis Prima</td>
      <td>Bruce Reitherman</td>
      <td>166409</td>
      <td>141843612</td>
    </tr>
    <tr>
      <th>993</th>
      <td>Blowup</td>
      <td>1966</td>
      <td>A</td>
      <td>111</td>
      <td>Drama, Mystery, Thriller</td>
      <td>7.6</td>
      <td>A fashion photographer unknowingly captures a ...</td>
      <td>82.00000</td>
      <td>Michelangelo Antonioni</td>
      <td>David Hemmings</td>
      <td>Vanessa Redgrave</td>
      <td>Sarah Miles</td>
      <td>John Castle</td>
      <td>56513</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>994</th>
      <td>A Hard Day's Night</td>
      <td>1964</td>
      <td>U</td>
      <td>87</td>
      <td>Comedy, Music, Musical</td>
      <td>7.6</td>
      <td>Over two "typical" days in the life of The Bea...</td>
      <td>96.00000</td>
      <td>Richard Lester</td>
      <td>John Lennon</td>
      <td>Paul McCartney</td>
      <td>George Harrison</td>
      <td>Ringo Starr</td>
      <td>40351</td>
      <td>13780024</td>
    </tr>
    <tr>
      <th>995</th>
      <td>Breakfast at Tiffany's</td>
      <td>1961</td>
      <td>A</td>
      <td>115</td>
      <td>Comedy, Drama, Romance</td>
      <td>7.6</td>
      <td>A young New York socialite becomes interested ...</td>
      <td>76.00000</td>
      <td>Blake Edwards</td>
      <td>Audrey Hepburn</td>
      <td>George Peppard</td>
      <td>Patricia Neal</td>
      <td>Buddy Ebsen</td>
      <td>166544</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>996</th>
      <td>Giant</td>
      <td>1956</td>
      <td>G</td>
      <td>201</td>
      <td>Drama, Western</td>
      <td>7.6</td>
      <td>Sprawling epic covering the life of a Texas ca...</td>
      <td>84.00000</td>
      <td>George Stevens</td>
      <td>Elizabeth Taylor</td>
      <td>Rock Hudson</td>
      <td>James Dean</td>
      <td>Carroll Baker</td>
      <td>34075</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>997</th>
      <td>From Here to Eternity</td>
      <td>1953</td>
      <td>Passed</td>
      <td>118</td>
      <td>Drama, Romance, War</td>
      <td>7.6</td>
      <td>In Hawaii in 1941, a private is cruelly punish...</td>
      <td>85.00000</td>
      <td>Fred Zinnemann</td>
      <td>Burt Lancaster</td>
      <td>Montgomery Clift</td>
      <td>Deborah Kerr</td>
      <td>Donna Reed</td>
      <td>43374</td>
      <td>30500000</td>
    </tr>
    <tr>
      <th>998</th>
      <td>Lifeboat</td>
      <td>1944</td>
      <td>Unknown</td>
      <td>97</td>
      <td>Drama, War</td>
      <td>7.6</td>
      <td>Several survivors of a torpedoed merchant ship...</td>
      <td>78.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Tallulah Bankhead</td>
      <td>John Hodiak</td>
      <td>Walter Slezak</td>
      <td>William Bendix</td>
      <td>26471</td>
      <td>23530892</td>
    </tr>
    <tr>
      <th>999</th>
      <td>The 39 Steps</td>
      <td>1935</td>
      <td>Unknown</td>
      <td>86</td>
      <td>Crime, Mystery, Thriller</td>
      <td>7.6</td>
      <td>A man in London tries to help a counter-espion...</td>
      <td>93.00000</td>
      <td>Alfred Hitchcock</td>
      <td>Robert Donat</td>
      <td>Madeleine Carroll</td>
      <td>Lucie Mannheim</td>
      <td>Godfrey Tearle</td>
      <td>51853</td>
      <td>23530892</td>
    </tr>
  </tbody>
</table>
</div>
    <div class="colab-df-buttons">

  <div class="colab-df-container">
    <button class="colab-df-convert" onclick="convertToInteractive('df-ca33b6c3-969b-4742-b2ec-ea067f6317fe')"
            title="Convert this dataframe to an interactive table."
            style="display:none;">

  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960">
    <path d="M120-120v-720h720v720H120Zm60-500h600v-160H180v160Zm220 220h160v-160H400v160Zm0 220h160v-160H400v160ZM180-400h160v-160H180v160Zm440 0h160v-160H620v160ZM180-180h160v-160H180v160Zm440 0h160v-160H620v160Z"/>
  </svg>
    </button>

  <style>
    .colab-df-container {
      display:flex;
      gap: 12px;
    }

    .colab-df-convert {
      background-color: #E8F0FE;
      border: none;
      border-radius: 50%;
      cursor: pointer;
      display: none;
      fill: #1967D2;
      height: 32px;
      padding: 0 0 0 0;
      width: 32px;
    }

    .colab-df-convert:hover {
      background-color: #E2EBFA;
      box-shadow: 0px 1px 2px rgba(60, 64, 67, 0.3), 0px 1px 3px 1px rgba(60, 64, 67, 0.15);
      fill: #174EA6;
    }

    .colab-df-buttons div {
      margin-bottom: 4px;
    }

    [theme=dark] .colab-df-convert {
      background-color: #3B4455;
      fill: #D2E3FC;
    }

    [theme=dark] .colab-df-convert:hover {
      background-color: #434B5C;
      box-shadow: 0px 1px 3px 1px rgba(0, 0, 0, 0.15);
      filter: drop-shadow(0px 1px 2px rgba(0, 0, 0, 0.3));
      fill: #FFFFFF;
    }
  </style>

    <script>
      const buttonEl =
        document.querySelector('#df-ca33b6c3-969b-4742-b2ec-ea067f6317fe button.colab-df-convert');
      buttonEl.style.display =
        google.colab.kernel.accessAllowed ? 'block' : 'none';

      async function convertToInteractive(key) {
        const element = document.querySelector('#df-ca33b6c3-969b-4742-b2ec-ea067f6317fe');
        const dataTable =
          await google.colab.kernel.invokeFunction('convertToInteractive',
                                                    [key], {});
        if (!dataTable) return;

        const docLinkHtml = 'Like what you see? Visit the ' +
          '<a target="_blank" href=https://colab.research.google.com/notebooks/data_table.ipynb>data table notebook</a>'
          + ' to learn more about interactive tables.';
        element.innerHTML = '';
        dataTable['output_type'] = 'display_data';
        await google.colab.output.renderOutput(dataTable, element);
        const docLink = document.createElement('div');
        docLink.innerHTML = docLinkHtml;
        element.appendChild(docLink);
      }
    </script>
  </div>


    <div id="df-d3d39f20-02da-4b59-8d46-d02e2698d78d">
      <button class="colab-df-quickchart" onclick="quickchart('df-d3d39f20-02da-4b59-8d46-d02e2698d78d')"
                title="Suggest charts"
                style="display:none;">

<svg xmlns="http://www.w3.org/2000/svg" height="24px"viewBox="0 0 24 24"
     width="24px">
    <g>
        <path d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zM9 17H7v-7h2v7zm4 0h-2V7h2v10zm4 0h-2v-4h2v4z"/>
    </g>
</svg>
      </button>

<style>
  .colab-df-quickchart {
      --bg-color: #E8F0FE;
      --fill-color: #1967D2;
      --hover-bg-color: #E2EBFA;
      --hover-fill-color: #174EA6;
      --disabled-fill-color: #AAA;
      --disabled-bg-color: #DDD;
  }

  [theme=dark] .colab-df-quickchart {
      --bg-color: #3B4455;
      --fill-color: #D2E3FC;
      --hover-bg-color: #434B5C;
      --hover-fill-color: #FFFFFF;
      --disabled-bg-color: #3B4455;
      --disabled-fill-color: #666;
  }

  .colab-df-quickchart {
    background-color: var(--bg-color);
    border: none;
    border-radius: 50%;
    cursor: pointer;
    display: none;
    fill: var(--fill-color);
    height: 32px;
    padding: 0;
    width: 32px;
  }

  .colab-df-quickchart:hover {
    background-color: var(--hover-bg-color);
    box-shadow: 0 1px 2px rgba(60, 64, 67, 0.3), 0 1px 3px 1px rgba(60, 64, 67, 0.15);
    fill: var(--button-hover-fill-color);
  }

  .colab-df-quickchart-complete:disabled,
  .colab-df-quickchart-complete:disabled:hover {
    background-color: var(--disabled-bg-color);
    fill: var(--disabled-fill-color);
    box-shadow: none;
  }

  .colab-df-spinner {
    border: 2px solid var(--fill-color);
    border-color: transparent;
    border-bottom-color: var(--fill-color);
    animation:
      spin 1s steps(1) infinite;
  }

  @keyframes spin {
    0% {
      border-color: transparent;
      border-bottom-color: var(--fill-color);
      border-left-color: var(--fill-color);
    }
    20% {
      border-color: transparent;
      border-left-color: var(--fill-color);
      border-top-color: var(--fill-color);
    }
    30% {
      border-color: transparent;
      border-left-color: var(--fill-color);
      border-top-color: var(--fill-color);
      border-right-color: var(--fill-color);
    }
    40% {
      border-color: transparent;
      border-right-color: var(--fill-color);
      border-top-color: var(--fill-color);
    }
    60% {
      border-color: transparent;
      border-right-color: var(--fill-color);
    }
    80% {
      border-color: transparent;
      border-right-color: var(--fill-color);
      border-bottom-color: var(--fill-color);
    }
    90% {
      border-color: transparent;
      border-bottom-color: var(--fill-color);
    }
  }
</style>

      <script>
        async function quickchart(key) {
          const quickchartButtonEl =
            document.querySelector('#' + key + ' button');
          quickchartButtonEl.disabled = true;  // To prevent multiple clicks.
          quickchartButtonEl.classList.add('colab-df-spinner');
          try {
            const charts = await google.colab.kernel.invokeFunction(
                'suggestCharts', [key], {});
          } catch (error) {
            console.error('Error during call to suggestCharts:', error);
          }
          quickchartButtonEl.classList.remove('colab-df-spinner');
          quickchartButtonEl.classList.add('colab-df-quickchart-complete');
        }
        (() => {
          let quickchartButtonEl =
            document.querySelector('#df-d3d39f20-02da-4b59-8d46-d02e2698d78d button');
          quickchartButtonEl.style.display =
            google.colab.kernel.accessAllowed ? 'block' : 'none';
        })();
      </script>
    </div>

  <div id="id_b34ff313-73c4-4186-9f52-2b806386cd5d">
    <style>
      .colab-df-generate {
        background-color: #E8F0FE;
        border: none;
        border-radius: 50%;
        cursor: pointer;
        display: none;
        fill: #1967D2;
        height: 32px;
        padding: 0 0 0 0;
        width: 32px;
      }

      .colab-df-generate:hover {
        background-color: #E2EBFA;
        box-shadow: 0px 1px 2px rgba(60, 64, 67, 0.3), 0px 1px 3px 1px rgba(60, 64, 67, 0.15);
        fill: #174EA6;
      }

      [theme=dark] .colab-df-generate {
        background-color: #3B4455;
        fill: #D2E3FC;
      }

      [theme=dark] .colab-df-generate:hover {
        background-color: #434B5C;
        box-shadow: 0px 1px 3px 1px rgba(0, 0, 0, 0.15);
        filter: drop-shadow(0px 1px 2px rgba(0, 0, 0, 0.3));
        fill: #FFFFFF;
      }
    </style>
    <button class="colab-df-generate" onclick="generateWithVariable('df')"
            title="Generate code using this dataframe."
            style="display:none;">

  <svg xmlns="http://www.w3.org/2000/svg" height="24px"viewBox="0 0 24 24"
       width="24px">
    <path d="M7,19H8.4L18.45,9,17,7.55,7,17.6ZM5,21V16.75L18.45,3.32a2,2,0,0,1,2.83,0l1.4,1.43a1.91,1.91,0,0,1,.58,1.4,1.91,1.91,0,0,1-.58,1.4L9.25,21ZM18.45,9,17,7.55Zm-12,3A5.31,5.31,0,0,0,4.9,8.1,5.31,5.31,0,0,0,1,6.5,5.31,5.31,0,0,0,4.9,4.9,5.31,5.31,0,0,0,6.5,1,5.31,5.31,0,0,0,8.1,4.9,5.31,5.31,0,0,0,12,6.5,5.46,5.46,0,0,0,6.5,12Z"/>
  </svg>
    </button>
    <script>
      (() => {
      const buttonEl =
        document.querySelector('#id_b34ff313-73c4-4186-9f52-2b806386cd5d button.colab-df-generate');
      buttonEl.style.display =
        google.colab.kernel.accessAllowed ? 'block' : 'none';

      buttonEl.onclick = () => {
        google.colab.notebook.generateWithVariable('df');
      }
      })();
    </script>
  </div>

    </div>
  </div>




# yoxlama(netice)


```python

df.info()
df.head()
# Sütunların tipləri
print(df_clean.dtypes)

# Boş olan dəyərlərin sayı
print(df_clean.isna().sum())


```

    <class 'pandas.core.frame.DataFrame'>
    Index: 999 entries, 0 to 999
    Data columns (total 15 columns):
     #   Column         Non-Null Count  Dtype  
    ---  ------         --------------  -----  
     0   Series_Title   999 non-null    object 
     1   Released_Year  999 non-null    Int64  
     2   Certificate    999 non-null    object 
     3   Runtime        999 non-null    int64  
     4   Genre          999 non-null    object 
     5   IMDB_Rating    999 non-null    float64
     6   Overview       999 non-null    object 
     7   Meta_score     999 non-null    float64
     8   Director       999 non-null    object 
     9   Star1          999 non-null    object 
     10  Star2          999 non-null    object 
     11  Star3          999 non-null    object 
     12  Star4          999 non-null    object 
     13  No_of_Votes    999 non-null    int64  
     14  Gross          999 non-null    float64
    dtypes: Int64(1), float64(3), int64(2), object(9)
    memory usage: 125.9+ KB



    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    /tmp/ipython-input-27-3104018243.py in <cell line: 0>()
          2 df.head()
          3 # Sütunların tipləri
    ----> 4 print(df_clean.dtypes)
          5 
          6 # Boş olan dəyərlərin sayı


    NameError: name 'df_clean' is not defined



```python
df["Released_Year"] = pd.to_numeric(df["Released_Year"], errors="coerce").astype("Int64")
```

# EDA — İlkin Məlumat Analizi


# Rəqəmsal Sütunlar Arasında Korrelyasiya Matrisi


```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.heatmap(
    df_clean[["IMDB_Rating", "Meta_score", "No_of_Votes", "Gross", "Runtime"]].corr(),
    annot=True, cmap='coolwarm'
)
plt.title(" Rəqəmsal Sütunlar Arasında Korrelyasiya Matrisi")
plt.show()

```


    
![png](output_9_0.png)
    


# IMDb Reytinqlərinin Paylanması


```python
sns.histplot(df_clean["IMDB_Rating"], bins=20, kde=True)
plt.title(" IMDb Reytinqlərinin Paylanması")
plt.xlabel("IMDb Reytinqi")
plt.ylabel("Film sayı")
plt.show()

```


    
![png](output_11_0.png)
    




# Ən Populyar 10 Janr


```python
import plotly.express as px
import pandas as pd

# Janrları parçalayırıq və ən çox rast gəlinən 10 janrı seçirik
top_genres = df_clean["Genre"].str.split(", ").explode().value_counts().head(10).reset_index()
top_genres.columns = ["Genre", "Count"]

# Interaktiv bar chart (rəngli və hover funksiyalı)
fig = px.bar(
    top_genres,
    x="Genre",
    y="Count",
    color="Count",
    color_continuous_scale="deep",  # Alternativlər: magma, viridis, plasma, turbo, cividis
    title="🎭 Ən Populyar 10 Janr"
)

# Qrafik parametrləri
fig.update_layout(
    template="plotly_white",
    title_font_size=20,
    xaxis_title="Janr",
    yaxis_title="Film sayı",
    xaxis_tickangle=-45
)

fig.show()


```


<html>
<head><meta charset="utf-8" /></head>
<body>
    <div>            <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/MathJax.js?config=TeX-AMS-MML_SVG"></script><script type="text/javascript">if (window.MathJax && window.MathJax.Hub && window.MathJax.Hub.Config) {window.MathJax.Hub.Config({SVG: {font: "STIX-Web"}});}</script>                <script type="text/javascript">window.PlotlyConfig = {MathJaxConfig: 'local'};</script>
        <script charset="utf-8" src="https://cdn.plot.ly/plotly-2.35.2.min.js"></script>                <div id="342b9d3f-26ab-4fcf-9b98-45fbd1799825" class="plotly-graph-div" style="height:525px; width:100%;"></div>            <script type="text/javascript">                                    window.PLOTLYENV=window.PLOTLYENV || {};                                    if (document.getElementById("342b9d3f-26ab-4fcf-9b98-45fbd1799825")) {                    Plotly.newPlot(                        "342b9d3f-26ab-4fcf-9b98-45fbd1799825",                        [{"alignmentgroup":"True","hovertemplate":"Genre=%{x}\u003cbr\u003eCount=%{marker.color}\u003cextra\u003e\u003c\u002fextra\u003e","legendgroup":"","marker":{"color":[723,233,209,195,189,137,125,109,99,82],"coloraxis":"coloraxis","pattern":{"shape":""}},"name":"","offsetgroup":"","orientation":"v","showlegend":false,"textposition":"auto","x":["Drama","Comedy","Crime","Adventure","Action","Thriller","Romance","Biography","Mystery","Animation"],"xaxis":"x","y":[723,233,209,195,189,137,125,109,99,82],"yaxis":"y","type":"bar"}],                        {"template":{"data":{"barpolar":[{"marker":{"line":{"color":"white","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"barpolar"}],"bar":[{"error_x":{"color":"#2a3f5f"},"error_y":{"color":"#2a3f5f"},"marker":{"line":{"color":"white","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"bar"}],"carpet":[{"aaxis":{"endlinecolor":"#2a3f5f","gridcolor":"#C8D4E3","linecolor":"#C8D4E3","minorgridcolor":"#C8D4E3","startlinecolor":"#2a3f5f"},"baxis":{"endlinecolor":"#2a3f5f","gridcolor":"#C8D4E3","linecolor":"#C8D4E3","minorgridcolor":"#C8D4E3","startlinecolor":"#2a3f5f"},"type":"carpet"}],"choropleth":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"choropleth"}],"contourcarpet":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"contourcarpet"}],"contour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"contour"}],"heatmapgl":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmapgl"}],"heatmap":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmap"}],"histogram2dcontour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2dcontour"}],"histogram2d":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2d"}],"histogram":[{"marker":{"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"histogram"}],"mesh3d":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"mesh3d"}],"parcoords":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"parcoords"}],"pie":[{"automargin":true,"type":"pie"}],"scatter3d":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatter3d"}],"scattercarpet":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattercarpet"}],"scattergeo":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergeo"}],"scattergl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergl"}],"scattermapbox":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattermapbox"}],"scatterpolargl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolargl"}],"scatterpolar":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolar"}],"scatter":[{"fillpattern":{"fillmode":"overlay","size":10,"solidity":0.2},"type":"scatter"}],"scatterternary":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterternary"}],"surface":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"surface"}],"table":[{"cells":{"fill":{"color":"#EBF0F8"},"line":{"color":"white"}},"header":{"fill":{"color":"#C8D4E3"},"line":{"color":"white"}},"type":"table"}]},"layout":{"annotationdefaults":{"arrowcolor":"#2a3f5f","arrowhead":0,"arrowwidth":1},"autotypenumbers":"strict","coloraxis":{"colorbar":{"outlinewidth":0,"ticks":""}},"colorscale":{"diverging":[[0,"#8e0152"],[0.1,"#c51b7d"],[0.2,"#de77ae"],[0.3,"#f1b6da"],[0.4,"#fde0ef"],[0.5,"#f7f7f7"],[0.6,"#e6f5d0"],[0.7,"#b8e186"],[0.8,"#7fbc41"],[0.9,"#4d9221"],[1,"#276419"]],"sequential":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"sequentialminus":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]]},"colorway":["#636efa","#EF553B","#00cc96","#ab63fa","#FFA15A","#19d3f3","#FF6692","#B6E880","#FF97FF","#FECB52"],"font":{"color":"#2a3f5f"},"geo":{"bgcolor":"white","lakecolor":"white","landcolor":"white","showlakes":true,"showland":true,"subunitcolor":"#C8D4E3"},"hoverlabel":{"align":"left"},"hovermode":"closest","mapbox":{"style":"light"},"paper_bgcolor":"white","plot_bgcolor":"white","polar":{"angularaxis":{"gridcolor":"#EBF0F8","linecolor":"#EBF0F8","ticks":""},"bgcolor":"white","radialaxis":{"gridcolor":"#EBF0F8","linecolor":"#EBF0F8","ticks":""}},"scene":{"xaxis":{"backgroundcolor":"white","gridcolor":"#DFE8F3","gridwidth":2,"linecolor":"#EBF0F8","showbackground":true,"ticks":"","zerolinecolor":"#EBF0F8"},"yaxis":{"backgroundcolor":"white","gridcolor":"#DFE8F3","gridwidth":2,"linecolor":"#EBF0F8","showbackground":true,"ticks":"","zerolinecolor":"#EBF0F8"},"zaxis":{"backgroundcolor":"white","gridcolor":"#DFE8F3","gridwidth":2,"linecolor":"#EBF0F8","showbackground":true,"ticks":"","zerolinecolor":"#EBF0F8"}},"shapedefaults":{"line":{"color":"#2a3f5f"}},"ternary":{"aaxis":{"gridcolor":"#DFE8F3","linecolor":"#A2B1C6","ticks":""},"baxis":{"gridcolor":"#DFE8F3","linecolor":"#A2B1C6","ticks":""},"bgcolor":"white","caxis":{"gridcolor":"#DFE8F3","linecolor":"#A2B1C6","ticks":""}},"title":{"x":0.05},"xaxis":{"automargin":true,"gridcolor":"#EBF0F8","linecolor":"#EBF0F8","ticks":"","title":{"standoff":15},"zerolinecolor":"#EBF0F8","zerolinewidth":2},"yaxis":{"automargin":true,"gridcolor":"#EBF0F8","linecolor":"#EBF0F8","ticks":"","title":{"standoff":15},"zerolinecolor":"#EBF0F8","zerolinewidth":2}}},"xaxis":{"anchor":"y","domain":[0.0,1.0],"title":{"text":"Janr"},"tickangle":-45},"yaxis":{"anchor":"x","domain":[0.0,1.0],"title":{"text":"Film sayı"}},"coloraxis":{"colorbar":{"title":{"text":"Count"}},"colorscale":[[0.0,"rgb(253, 253, 204)"],[0.09090909090909091,"rgb(206, 236, 179)"],[0.18181818181818182,"rgb(156, 219, 165)"],[0.2727272727272727,"rgb(111, 201, 163)"],[0.36363636363636365,"rgb(86, 177, 163)"],[0.45454545454545453,"rgb(76, 153, 160)"],[0.5454545454545454,"rgb(68, 130, 155)"],[0.6363636363636364,"rgb(62, 108, 150)"],[0.7272727272727273,"rgb(62, 82, 143)"],[0.8181818181818182,"rgb(64, 60, 115)"],[0.9090909090909091,"rgb(54, 43, 77)"],[1.0,"rgb(39, 26, 44)"]]},"legend":{"tracegroupgap":0},"title":{"text":"🎭 Ən Populyar 10 Janr","font":{"size":20}},"barmode":"relative"},                        {"responsive": true}                    ).then(function(){

var gd = document.getElementById('342b9d3f-26ab-4fcf-9b98-45fbd1799825');
var x = new MutationObserver(function (mutations, observer) {{
        var display = window.getComputedStyle(gd).display;
        if (!display || display === 'none') {{
            console.log([gd, 'removed!']);
            Plotly.purge(gd);
            observer.disconnect();
        }}
}});

// Listen for the removal of the full notebook cells
var notebookContainer = gd.closest('#notebook-container');
if (notebookContainer) {{
    x.observe(notebookContainer, {childList: true});
}}

// Listen for the clearing of the current output cell
var outputEl = gd.closest('.output');
if (outputEl) {{
    x.observe(outputEl, {childList: true});
}}

                        })                };                            </script>        </div>
</body>
</html>


# 🎬 1. IMDb Reytinqlərinə görə Ən Yüksək 10 Film


```python
import plotly.express as px

top10_rating = df_clean.sort_values(by="IMDB_Rating", ascending=False).head(10)

fig = px.bar(
    top10_rating,
    x="IMDB_Rating",
    y="Series_Title",
    orientation="h",
    color="IMDB_Rating",
    color_continuous_scale="viridis",
    title="🌟 IMDb Reytinqinə görə TOP 10 Film",
    labels={"IMDB_Rating": "IMDb Reytinqi", "Series_Title": "Film"}
)

fig.update_layout(
    template="plotly_white",
    yaxis={"categoryorder": "total ascending"},
    title_font_size=20
)

fig.show()


```


<html>
<head><meta charset="utf-8" /></head>
<body>
    <div>            <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/MathJax.js?config=TeX-AMS-MML_SVG"></script><script type="text/javascript">if (window.MathJax && window.MathJax.Hub && window.MathJax.Hub.Config) {window.MathJax.Hub.Config({SVG: {font: "STIX-Web"}});}</script>                <script type="text/javascript">window.PlotlyConfig = {MathJaxConfig: 'local'};</script>
        <script charset="utf-8" src="https://cdn.plot.ly/plotly-2.35.2.min.js"></script>                <div id="41dc732e-c047-4cb3-89e4-c46171a1325d" class="plotly-graph-div" style="height:525px; width:100%;"></div>            <script type="text/javascript">                                    window.PLOTLYENV=window.PLOTLYENV || {};                                    if (document.getElementById("41dc732e-c047-4cb3-89e4-c46171a1325d")) {                    Plotly.newPlot(                        "41dc732e-c047-4cb3-89e4-c46171a1325d",                        [{"alignmentgroup":"True","hovertemplate":"IMDb Reytinqi=%{marker.color}\u003cbr\u003eFilm=%{y}\u003cextra\u003e\u003c\u002fextra\u003e","legendgroup":"","marker":{"color":[9.3,9.2,9.0,9.0,9.0,8.9,8.9,8.9,8.8,8.8],"coloraxis":"coloraxis","pattern":{"shape":""}},"name":"","offsetgroup":"","orientation":"h","showlegend":false,"textposition":"auto","x":[9.3,9.2,9.0,9.0,9.0,8.9,8.9,8.9,8.8,8.8],"xaxis":"x","y":["The Shawshank Redemption","The Godfather","12 Angry Men","The Dark Knight","The Godfather: Part II","The Lord of the Rings: The Return of the King","Schindler's List","Pulp Fiction","Inception","Il buono, il brutto, il cattivo"],"yaxis":"y","type":"bar"}],                        {"template":{"data":{"barpolar":[{"marker":{"line":{"color":"white","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"barpolar"}],"bar":[{"error_x":{"color":"#2a3f5f"},"error_y":{"color":"#2a3f5f"},"marker":{"line":{"color":"white","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"bar"}],"carpet":[{"aaxis":{"endlinecolor":"#2a3f5f","gridcolor":"#C8D4E3","linecolor":"#C8D4E3","minorgridcolor":"#C8D4E3","startlinecolor":"#2a3f5f"},"baxis":{"endlinecolor":"#2a3f5f","gridcolor":"#C8D4E3","linecolor":"#C8D4E3","minorgridcolor":"#C8D4E3","startlinecolor":"#2a3f5f"},"type":"carpet"}],"choropleth":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"choropleth"}],"contourcarpet":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"contourcarpet"}],"contour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"contour"}],"heatmapgl":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmapgl"}],"heatmap":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmap"}],"histogram2dcontour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2dcontour"}],"histogram2d":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2d"}],"histogram":[{"marker":{"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"histogram"}],"mesh3d":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"mesh3d"}],"parcoords":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"parcoords"}],"pie":[{"automargin":true,"type":"pie"}],"scatter3d":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatter3d"}],"scattercarpet":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattercarpet"}],"scattergeo":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergeo"}],"scattergl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergl"}],"scattermapbox":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattermapbox"}],"scatterpolargl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolargl"}],"scatterpolar":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolar"}],"scatter":[{"fillpattern":{"fillmode":"overlay","size":10,"solidity":0.2},"type":"scatter"}],"scatterternary":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterternary"}],"surface":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"surface"}],"table":[{"cells":{"fill":{"color":"#EBF0F8"},"line":{"color":"white"}},"header":{"fill":{"color":"#C8D4E3"},"line":{"color":"white"}},"type":"table"}]},"layout":{"annotationdefaults":{"arrowcolor":"#2a3f5f","arrowhead":0,"arrowwidth":1},"autotypenumbers":"strict","coloraxis":{"colorbar":{"outlinewidth":0,"ticks":""}},"colorscale":{"diverging":[[0,"#8e0152"],[0.1,"#c51b7d"],[0.2,"#de77ae"],[0.3,"#f1b6da"],[0.4,"#fde0ef"],[0.5,"#f7f7f7"],[0.6,"#e6f5d0"],[0.7,"#b8e186"],[0.8,"#7fbc41"],[0.9,"#4d9221"],[1,"#276419"]],"sequential":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"sequentialminus":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]]},"colorway":["#636efa","#EF553B","#00cc96","#ab63fa","#FFA15A","#19d3f3","#FF6692","#B6E880","#FF97FF","#FECB52"],"font":{"color":"#2a3f5f"},"geo":{"bgcolor":"white","lakecolor":"white","landcolor":"white","showlakes":true,"showland":true,"subunitcolor":"#C8D4E3"},"hoverlabel":{"align":"left"},"hovermode":"closest","mapbox":{"style":"light"},"paper_bgcolor":"white","plot_bgcolor":"white","polar":{"angularaxis":{"gridcolor":"#EBF0F8","linecolor":"#EBF0F8","ticks":""},"bgcolor":"white","radialaxis":{"gridcolor":"#EBF0F8","linecolor":"#EBF0F8","ticks":""}},"scene":{"xaxis":{"backgroundcolor":"white","gridcolor":"#DFE8F3","gridwidth":2,"linecolor":"#EBF0F8","showbackground":true,"ticks":"","zerolinecolor":"#EBF0F8"},"yaxis":{"backgroundcolor":"white","gridcolor":"#DFE8F3","gridwidth":2,"linecolor":"#EBF0F8","showbackground":true,"ticks":"","zerolinecolor":"#EBF0F8"},"zaxis":{"backgroundcolor":"white","gridcolor":"#DFE8F3","gridwidth":2,"linecolor":"#EBF0F8","showbackground":true,"ticks":"","zerolinecolor":"#EBF0F8"}},"shapedefaults":{"line":{"color":"#2a3f5f"}},"ternary":{"aaxis":{"gridcolor":"#DFE8F3","linecolor":"#A2B1C6","ticks":""},"baxis":{"gridcolor":"#DFE8F3","linecolor":"#A2B1C6","ticks":""},"bgcolor":"white","caxis":{"gridcolor":"#DFE8F3","linecolor":"#A2B1C6","ticks":""}},"title":{"x":0.05},"xaxis":{"automargin":true,"gridcolor":"#EBF0F8","linecolor":"#EBF0F8","ticks":"","title":{"standoff":15},"zerolinecolor":"#EBF0F8","zerolinewidth":2},"yaxis":{"automargin":true,"gridcolor":"#EBF0F8","linecolor":"#EBF0F8","ticks":"","title":{"standoff":15},"zerolinecolor":"#EBF0F8","zerolinewidth":2}}},"xaxis":{"anchor":"y","domain":[0.0,1.0],"title":{"text":"IMDb Reytinqi"}},"yaxis":{"anchor":"x","domain":[0.0,1.0],"title":{"text":"Film"},"categoryorder":"total ascending"},"coloraxis":{"colorbar":{"title":{"text":"IMDb Reytinqi"}},"colorscale":[[0.0,"#440154"],[0.1111111111111111,"#482878"],[0.2222222222222222,"#3e4989"],[0.3333333333333333,"#31688e"],[0.4444444444444444,"#26828e"],[0.5555555555555556,"#1f9e89"],[0.6666666666666666,"#35b779"],[0.7777777777777778,"#6ece58"],[0.8888888888888888,"#b5de2b"],[1.0,"#fde725"]]},"legend":{"tracegroupgap":0},"title":{"text":"🌟 IMDb Reytinqinə görə TOP 10 Film","font":{"size":20}},"barmode":"relative"},                        {"responsive": true}                    ).then(function(){

var gd = document.getElementById('41dc732e-c047-4cb3-89e4-c46171a1325d');
var x = new MutationObserver(function (mutations, observer) {{
        var display = window.getComputedStyle(gd).display;
        if (!display || display === 'none') {{
            console.log([gd, 'removed!']);
            Plotly.purge(gd);
            observer.disconnect();
        }}
}});

// Listen for the removal of the full notebook cells
var notebookContainer = gd.closest('#notebook-container');
if (notebookContainer) {{
    x.observe(notebookContainer, {childList: true});
}}

// Listen for the clearing of the current output cell
var outputEl = gd.closest('.output');
if (outputEl) {{
    x.observe(outputEl, {childList: true});
}}

                        })                };                            </script>        </div>
</body>
</html>


# 🎬 Ən Çox Filmə Sahib 10 Rejissor


```python
import seaborn as sns
import matplotlib.pyplot as plt

# Rejissorların film sayı
top_directors = df_clean["Director"].value_counts().head(10)

# Rəng palitrası: "viridis", "mako", "rocket", "coolwarm" kimi modern seçimlər mümkündür
sns.barplot(
    x=top_directors.values,
    y=top_directors.index,
    palette="mako"  # rəng palitrası burada dəyişdirilə bilər
)

plt.title(" Ən Çox Filmə Sahib 10 Rejissor", fontsize=14, fontweight='bold')
plt.xlabel("Film sayı", fontsize=12)
plt.ylabel("Rejissor", fontsize=12)
plt.xticks(fontsize=10)
plt.yticks(fontsize=10)
plt.grid(axis="x", linestyle="--", alpha=0.5)
plt.tight_layout()
plt.show()

```

    /tmp/ipython-input-25-1538661305.py:8: FutureWarning:
    
    
    
    Passing `palette` without assigning `hue` is deprecated and will be removed in v0.14.0. Assign the `y` variable to `hue` and set `legend=False` for the same effect.
    
    



    
![png](output_18_1.png)
    


## Ən yüksək IMDb Reytinqinə sahib aktyorlar (Star1)


```python
top_actors_rating = df_clean.groupby("Star1")["IMDB_Rating"].mean().sort_values(ascending=False).head(10)
sns.barplot(x=top_actors_rating.values, y=top_actors_rating.index, palette="magma")
plt.title(" Ən Yüksək Reytinqli 10 Aktyor (Star1)")
plt.xlabel("Orta IMDb Reytinqi")
plt.ylabel("Aktyor")
plt.tight_layout()
plt.show()
```

    /tmp/ipython-input-26-611418713.py:2: FutureWarning:
    
    
    
    Passing `palette` without assigning `hue` is deprecated and will be removed in v0.14.0. Assign the `y` variable to `hue` and set `legend=False` for the same effect.
    
    



    
![png](output_20_1.png)
    








# İllərə görə film sayı


```python
year_counts = df_clean["Released_Year"].value_counts().sort_index()
sns.lineplot(x=year_counts.index, y=year_counts.values, marker="o", color="teal")
plt.title(" İllərə görə Film Sayı")
plt.xlabel("İl")
plt.ylabel("Film sayı")
plt.grid(True)
plt.tight_layout()
plt.show()
```


    
![png](output_25_0.png)
    


# Ən yüksək gəlirə sahib 10 film


```python
top10_gross = df_clean.sort_values(by="Gross", ascending=False).head(10)
sns.barplot(x=top10_gross["Gross"], y=top10_gross["Series_Title"], palette="rocket")
plt.title(" Ən Yüksək Gəlirə Sahib 10 Film")
plt.xlabel("Gəlir (USD)")
plt.ylabel("Film")
plt.tight_layout()
plt.show()
```

    /tmp/ipython-input-27-1266620089.py:2: FutureWarning:
    
    
    
    Passing `palette` without assigning `hue` is deprecated and will be removed in v0.14.0. Assign the `y` variable to `hue` and set `legend=False` for the same effect.
    
    



    
![png](output_27_1.png)
    


# Janra görə orta gəlir (Gross)


```python
genre_gross = df_clean.copy()
genre_gross["Genre"] = genre_gross["Genre"].str.split(", ")
genre_gross = genre_gross.explode("Genre")
genre_gross["Genre"] = genre_gross["Genre"].str.strip()
avg_gross_by_genre = genre_gross.groupby("Genre")["Gross"].mean().sort_values(ascending=False).head(10)
sns.barplot(x=avg_gross_by_genre.values, y=avg_gross_by_genre.index, palette="viridis")
plt.title(" Janra görə Orta Gəlir (TOP 10)")
plt.xlabel("Orta Gəlir (USD)")
plt.ylabel("Janr")
plt.tight_layout()
plt.show()
```

    /tmp/ipython-input-28-1462833539.py:6: FutureWarning:
    
    
    
    Passing `palette` without assigning `hue` is deprecated and will be removed in v0.14.0. Assign the `y` variable to `hue` and set `legend=False` for the same effect.
    
    



    
![png](output_29_1.png)
    


zsx


```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Faylı oxuyuruq
df = pd.read_csv("/content/imdb_top_1000.csv")

# Ən çox baş rolda çəkilən aktyorlar
top_actors_by_count = df["Star1"].value_counts().head(10)

# Vizual qururuq
plt.figure(figsize=(10, 6))
sns.barplot(
    x=top_actors_by_count.values,
    y=top_actors_by_count.index,
    palette="rocket"
)
plt.title("🎬 Ən Çox Baş Rol Oynamış 10 Aktyor (Star1)")
plt.xlabel("Film sayı")
plt.ylabel("Aktyor")
plt.tight_layout()
plt.show()

```


    ---------------------------------------------------------------------------

    FileNotFoundError                         Traceback (most recent call last)

    /tmp/ipython-input-29-972539494.py in <cell line: 0>()
          4 
          5 # Faylı oxuyuruq
    ----> 6 df = pd.read_csv("/content/imdb_top_1000.csv")
          7 
          8 # Ən çox baş rolda çəkilən aktyorlar


    /usr/local/lib/python3.11/dist-packages/pandas/io/parsers/readers.py in read_csv(filepath_or_buffer, sep, delimiter, header, names, index_col, usecols, dtype, engine, converters, true_values, false_values, skipinitialspace, skiprows, skipfooter, nrows, na_values, keep_default_na, na_filter, verbose, skip_blank_lines, parse_dates, infer_datetime_format, keep_date_col, date_parser, date_format, dayfirst, cache_dates, iterator, chunksize, compression, thousands, decimal, lineterminator, quotechar, quoting, doublequote, escapechar, comment, encoding, encoding_errors, dialect, on_bad_lines, delim_whitespace, low_memory, memory_map, float_precision, storage_options, dtype_backend)
       1024     kwds.update(kwds_defaults)
       1025 
    -> 1026     return _read(filepath_or_buffer, kwds)
       1027 
       1028 


    /usr/local/lib/python3.11/dist-packages/pandas/io/parsers/readers.py in _read(filepath_or_buffer, kwds)
        618 
        619     # Create the parser.
    --> 620     parser = TextFileReader(filepath_or_buffer, **kwds)
        621 
        622     if chunksize or iterator:


    /usr/local/lib/python3.11/dist-packages/pandas/io/parsers/readers.py in __init__(self, f, engine, **kwds)
       1618 
       1619         self.handles: IOHandles | None = None
    -> 1620         self._engine = self._make_engine(f, self.engine)
       1621 
       1622     def close(self) -> None:


    /usr/local/lib/python3.11/dist-packages/pandas/io/parsers/readers.py in _make_engine(self, f, engine)
       1878                 if "b" not in mode:
       1879                     mode += "b"
    -> 1880             self.handles = get_handle(
       1881                 f,
       1882                 mode,


    /usr/local/lib/python3.11/dist-packages/pandas/io/common.py in get_handle(path_or_buf, mode, encoding, compression, memory_map, is_text, errors, storage_options)
        871         if ioargs.encoding and "b" not in ioargs.mode:
        872             # Encoding
    --> 873             handle = open(
        874                 handle,
        875                 ioargs.mode,


    FileNotFoundError: [Errno 2] No such file or directory: '/content/imdb_top_1000.csv'

