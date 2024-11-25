<script>
	import "../app.css";

	import { afterNavigate } from "$app/navigation";

	afterNavigate(() => {
		// Runs after navigating between pages
		// @ts-ignore : 모든 네비게이션 경로에서 flyonui 디자인을 적용하기 위한 코드. 타입 힌트가 올바르게 호출되지 않아 오류가 발생함.
		HSStaticMethods.autoInit();
	});
</script>

<slot></slot>
