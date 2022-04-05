<h3>Olá meu nome é</h3><h2>Arthur Rosa</h2> - :four_leaf_clover: <br>

-=-
<br>
	<div style="display: inline_block" align="center">
	<img align="center" alt="java" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" />
</div>


```java
@Controller
public class ArthurController extends Developer {

	@Autowired
	private ArthurRepository repArthur;

	@RequestMapping("aboutYou")
	public String aboutMe(Model model) {
    		Arthur art =  new Arthur();
    
    		art.setName(" Arthur Rosa ");
    		art.setEmail(" arthur.corporativo@outlook.com ");
    		art.setLinkedin(" https://www.linkedin.com/in/arthur-rosa-a2805b208/ ");
  
  		model.addAttribute("arthur", art);
		return "arthur/about";
	}

	@RequestMapping("languages")
	public String languages(Model model) {
		
		List<String> lang = new ArrayList<String>();
    
    		lang.add(" JavaScript ");
    		lang.add(" Php ");
    		lang.add(" Java ");
    		lang.add(" Sql ");
    		lang.add(" SpringBoot ");
    		lang.add(" Hibernate ");
    
		model.addAttribute("languages", lang);
		return "arthur/languages";
	}

}
```
<br>
 <div align="center" style="display: inline_block">
     <a href="https://github.com/ArthurCorpO">
     <img height="160em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ArthurCorpO&layout=compact&langs_count=7&theme=github_dark"/>
   </div>
