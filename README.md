# springboottask

springboot定时计划Demo
定时任务task

在启动类中SpringboottaskApplication.java中使用注解@EnableScheduling开启定时任务，会自动扫描

在你要执行定时计划的类中（比如我这里的task包下的TestTask.java），类上方定义@Component作为组件被容器扫描
在执行的方法中，添加@Scheduled(fixRate=3000)，定义每过3秒执行任务。
