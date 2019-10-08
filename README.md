# 第一次的作业
···
<?php 
	echo "<h1>第一题</h1>";
	$array_rand = array();
	for ($i=0; $i < 10; $i++) { 
		$array_rand[$i] = rand(10,100);
	}
	$assetsm = 0;
	$assetbig = 0;
	$assetaverage = 0;
	for ($i=0; $i < count($array_rand); $i++) { 
		echo "数值：".$array_rand[$i];
	}
	$i = 0;
	for ($i=0; $i < count($array_rand); $i++) { 
		if ($i == 0) {
			$assetbig = $array_rand[$i];
			$assetsm = $array_rand[$i];
		} elseif ($array_rand[$i] < $assetsm) {
			$assetsm = $array_rand[$i];
		} elseif ($array_rand[$i] > $assetbig) {
			$assetbig = $array_rand[$i];
		}
		$assetaverage = $array_rand[$i]+$assetaverage;

	}
	echo '<br>';
	echo "最大值:".$assetbig;
	echo "最小值：".$assetsm;
	echo "平均值：".$assetaverage/10;
	echo "<h1>第二题</h1>";
	$array_order = array(1,2,3,4,5,6,7,8);
	$i = 0;
	$asset_middle = array();
	for ($i=0; $i < count($array_order); $i++) { 
		$asset_middle[$i] = $array_order[count($array_order)-1-$i];
		echo "倒叙元素值：".$asset_middle[$i];
	}
	echo '<h1>第三题</h1>';
	$array_number_ = array();
	$i = 0;
	for ($i=0; $i < 20; $i++) {
		if ($i == 0) {
			$array_number_[$i] = 0;
		} else {
			$array_number_[$i] = 2*$i -1;
		}
		echo '输出：'.$array_number_[$i];
	}
?>
···
