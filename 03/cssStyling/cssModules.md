# CSS Modules
It different from stylesheets as we do not have to worry about name conflict here.
## create app.module.css file
```
.anime{
    color:red;
    font-size:20px;
}
```
## importing in component
```
import styles from './app.module.css'; 
const styleHandler=()=>{
    <div className={styles.anime}>Anime</div>
}
```